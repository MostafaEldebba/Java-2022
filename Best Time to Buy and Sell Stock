class Solution {
    public int maxProfit(int[] prices) {
        if (prices == null || prices.length <= 1) return 0;
        int profit = 0, n = prices.length;
        int[] min = new int[n];
        min[0] = prices[0];
        for (int i = 1; i < n; i++) {
            min[i] = Math.min(min[i - 1], prices[i]);
            profit = Math.max(profit, prices[i] - min[i]);
        }
        return profit;
    }
}
