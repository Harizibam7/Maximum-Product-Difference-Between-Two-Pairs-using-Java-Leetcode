![image](https://github.com/Harizibam7/Maximum-Product-Difference-Between-Two-Pairs-using-Java-Leetcode/assets/119025141/ada72389-f9f4-4c3c-83a6-a4c5cd0f7784)# Maximum-Product-Difference-Between-Two-Pairs-using-Java-Leetcode

    
    import java.util.*; 
    class Solution { 
        public int maxProductDifference(int[] nums) 
        { 
            int result = 0; 
            ArrayList<Integer> list = new ArrayList<Integer>(); 
            for(int i =0; i<nums.length;i++){ 
                    list.add(nums[i]); 
            } 
            Collections.sort(list); 
            result = (list.get(nums.length-2)*list.get(nums.length-1) ) - (list.get(0)*list.get(1)); 
            return result; 
        } 
    }

    class Solution { 
        public int maxProductDifference(int[] nums) 
        { 
            Arrays.sort(nums);
            return ((nums[nums.length-2]*nums[nums.length-1]) - (nums[0]*nums[1]));  
        } 
    }
