![image](https://github.com/user-attachments/assets/de3f2475-0ce6-45ec-a7be-cb1e86536c76)

---
# Code :



import java.util.* ;
import java.io.*; 
public class Solution {
	public static int findSecondLargest(int n, int[] arr) {
		Set<Integer> set = new HashSet<>();
		for(int i=0;i<arr.length;i++){
			set.add(arr[i]);
		}
		if(set.size()<2){
			return -1;
		}

		List<Integer> list = new ArrayList<>(set);
		Collections.sort(list);

		return list.get(list.size() - 2);
	}
}

## Status : All Test Cases Passed (8/8).
