class Solution {
    public int trap(int[] height) {
        
       
        int max = height[0];
        int n = height.length;
        int p1 = 0;
        int p2 = 0;
        int count = 0;
        for(int i=0;i<n;i++)
        {
            p1 += height[i];
            if((max < height[i]))
            {
                max = height[i];
            }
        }
        
        int area = max*n;
        int coun = 0;
        int start = height[0];
        int size = 0;
        for(int i=1;i<n;i++)
        {
            size++;
            if(start < height[i])
            {
                coun += (size*(max-start));
                size = 0;
                start = height[i];
            }
        }
        
        
        start = height[n-1];
        size = 0;
        int coun2 = 0;
        for(int i=n-2;i>=0;i--)
        {
            size++;
            if(start < height[i])
            {
                coun2 += (size*(max-start));
                size = 0;
                start = height[i];
            }
        }
        
        return (area-(coun2+coun+p1));
   
    }
}
