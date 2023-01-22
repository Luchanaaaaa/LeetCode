There are m jobs to schedule on n processors.     
A schedule is balanced if the difference between the number of jobs scheduled on any two neighboring processors does not exceed 1.      
The k<sup> th </sup> processor is the most efficient, and thus, the maximum number of jobs should be scheduled on that processor.     
Find the maximum number of jobs that can be scheduled on the k<sup> th </sup> processor, such that the overall schedule remains balanced.         
Note: Each processor must have at least one job scheduled Example Consider n=5, m=11, k=3. 
```java
package org.example;

public class weRideOA1 {
    public static void main(String[] args) {
        //int a = getMaximumJobs(5, 14, 2);
        System.out.println(getMaximumJobs(5, 11, 5));
        //4


    }
    static int getMaximumJobs (int n, int m, int k){
        // : number of processor
        // Visualization of how array builds up (for k = 2, n = 5, m = 16) in the above code
        // 1 1 1 1 1 --> Sum is less than m = 16 - OK
        // 1 2 1 1 1 --> Sum is less than m = 16 - OK
        // 2 3 2 1 1 --> Sum is less than m = 16 - OK
        // 3 4 3 2 1 --> Sum is less than m = 16 - OK
        // 4 5 4 3 2  ---> sum is 18, greater than m. Hence answer is previous value for kth element, which is 4

        k--;
        int arr [] = new int[n];
        for(int i = 0; i < n; i++ ) arr[i] = 1;
        int sum = n, maxjob = 1;

        while( ++sum <= m){
            maxjob = ++arr[k];
            System.out.print("pre");
            for(int i : arr){

                System.out.print(i+"  ");

            }
            System.out.println(" ");

            for(int i = k - 1; i >= 0; i--){
                if((arr[i + 1] - arr[i] ) > 1){
                    arr[i] ++;
                    sum ++;
                }
            }

            for(int i = k + 1; i < n; i++){
                if((arr[i -1] - arr[i]) > 1){
                    arr[i] ++;
                    sum ++;
                }
            }
            for(int i : arr){
                System.out.print(i+"  ");

            }
            System.out.println("sum = " +sum);
            System.out.println(" ");

        }


        return  maxjob;
    }
}


```
