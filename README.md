# diffrent-_sort-in-diffrent-languages
Please contribute for different sorting algorithms in whatever language you prefer.
// Insertion sort in java
import java.io.*; // for handling input/output
import java.util.*; // contains Collections framework


class Main {
	public static void sort(int[] arr){
		for(int i=1; i<arr.length; i++){
			int current = arr[i];
			int j=i-1;
			while(j>=0 && arr[j]>current){
				arr[j+1]=arr[j];
				j--;
			}
			arr[j+1]=current;
		}
	}
	public static void main (String[] args) {
		Scanner sc = new Scanner(System.in);
		int T = sc.nextInt();
		for(int i=0; i<T; i++){
			int N = sc.nextInt();
			int[] a = new int[N];
			for(int j=0; j<N; j++){
				a[j]= sc.nextInt();
			}
			sort(a);
			for(int item: a){
				System.out.print(item+" ");
			}
			System.out.println();
		}

                      
	}
}
