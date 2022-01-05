# bubbleSorting
This is an implementation of the bubble sort algorithm.


/*
Bubble sort = checking left and right adjacent element;
if right element is smaller, swap it to left;
here greatest number get swapped in first loop & located at end position of array
 */

    public static void main(String[] args) {
        /*
        scanner class can be used to take araay input
        */
        int[] a = {3,5,1,6,2,9,4,10,49,21,32};
        for(int element: a){
            System.out.print(element + " ");
        }
        System.out.println();
        
        int len = a.length;   //n

        boolean check = true;
        
        
/*
here n = array lenght which is (int len)
Descending form = n-1
to reduce the iteration. As greater numbers get sorted from (first) right to left.To reduce time n-1-i
boolean to check if swapping is happening inside loop (j)
if swapped once check is false;
otherwise check is true & loop break;
 */
 
 
        for(int i = 0; i < len-1-i;i++){
            for(int j = 0; j < len-1; j++){

                if(a[j+1] < a[j]){
                    int temp = a[j+1];
                    a[j+1] = a[j];
                    a[j] = temp;
                    check = false;
                }
            }
            if(check) break;
        }

// for-each loop to print sorted array
        for(int item: a){
            System.out.print(item + " ");
        }
    }

