# Maximum-Minimum-Element-in-an-array
Java code for Max &amp; Min 

public class MaxMinElement {
    public int maxElement(int[] arr){
        int max=0;
        int i=0;
        while (i<arr.length){
            if(max<arr[i]){
                max=arr[i];
            }
            i++;
        }
        return max;
    }
    public int minElement(int[] arr){
        int min=0;
        int i=0;
        while (i<arr.length){
            if(min>arr[i]){
                min=arr[i];
            }
            i++;
        }
        return min;
    }
}

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        System.out.println("Enter size of the Array");
        Scanner input = new Scanner(System.in);
        int size = input.nextInt();
        System.out.println("Enter Elements");
        int[] arr1= InputArrays.Input(size);

        MaxMinElement m= new MaxMinElement();
        int maxNum = m.maxElement(arr1);
        int minNum = m.minElement(arr1);

        System.out.println("Maximum Number: "+ maxNum);
        System.out.println("Minimum Number: "+ minNum);
    }
}
