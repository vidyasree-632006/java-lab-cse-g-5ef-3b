# java-lab-cse-g-5ef-3b
EXPERIMENT -3B
## EXPERIMENT-3B 
# implement binary  search logic mechanism 
source code 
JAVA 
```
(logicfile)
import java.util.Arrays;
 class Binarysearchlogic {
    void search(int[] a, int k) {
        Arrays.sort(a);
        System.out.println("After sorting: " + Arrays.toString(a));
        int p = Arrays.binarySearch(a, k);
        System.out.println(p >= 0 ? "Element " + k + " found at position " + (p + 1) : "Not found");
    }
}


(main file)
  
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner S= new Scanner(System.in);
System.out.print("Size:");
int[]arr = new int  [S.nextInt()];
System.out.println("Enter"+ arr.length+"Elements:");
for(int i=0 ; i<arr.length; i++)arr[i]=S.nextInt();
System.out.print("Search for:");
new Binarysearchlogic() .search(arr , S.nextInt());

    }
}
```
# output: 
![output of exp 3b](3b.png)
