# Row_with_maximum_one-gfg

class Solution {
    public int rowWithMax1s(int arr[][]) {
        // code here
        int count=0;
        int maxx=0;
        int row=-1;
        for(int i=0;i<arr.length;i++){
            count=0;
            for(int j=0;j<arr[0].length;j++){
                if(arr[i][j]==1){
                    count++;
                }
            }
            if(count>maxx){
                maxx=count;
                row=i;
            }
        }
        return row;
    }
}
