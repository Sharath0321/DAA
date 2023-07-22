package SelectionSortWithRandom;
import java.util.Arrays;
import java.util.Random;

public class selSortWithRand
{
	
	public static void selectionSort(int[] arr)
	{  
		for (int i=0; i<arr.length-1; i++)  
		{  
			int index = i;  
			for (int j = i + 1; j < arr.length; j++)
			{  
				if (arr[j] < arr[index])
				{  
					index = j;
				}  
			}
			int temp = arr[index];   
			arr[index] = arr[i];  
			arr[i] = temp;  
		}  
	}
	
	public static int[] generateRandomNumbers(int n)
	{
		int[] nums = new int[n];
		Random rand = new Random();
		for (int i=0; i<n; i++)
		{
			nums[i] = rand.nextInt(10000);
		}
		return nums;
	}
	
           
	public static void main(String[] args)
	{
		int[] nValues= {5000, 10000, 15000, 20000, 25000};
		long[] timeTaken = new long [nValues.length];
		for (int i = 0; i < nValues.length; i++)
		{
			int n = nValues[i];
			int[] arr = generateRandomNumbers(n);
			long startTime = System.nanoTime();
			selectionSort(arr);
			long endTime = System.nanoTime();
			long duration = (endTime-startTime)/100000;
			timeTaken[i] = duration;
			System.out.println("Time taken to start:" +n+ "Elements:" +duration+"Milliseconds:");
		
		}
	}
}
  
