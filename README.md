# hello-world
/*记录算法学习1*/
import java.util.Scanner;

public class page {

	public static void main(String[] args) {
		// TODO 自动生成的方法存根
		Scanner in = new Scanner(System.in);
		System.out.println("请输入页号：");
		int num = in.nextInt();
		int[] result = new int[10];
		for (int i = 1; i <= num; i++) {
			char[] arr = String.valueOf(i).toCharArray();//将i转换成字符型再放入字符数组arr中
			for (int j = 0; j < arr.length; j++) {
				int index = Integer.valueOf(arr[j] + "");
				result[index] = result[index] + 1;

			}
		}
		for (int i : result) {
			System.out.println(i);
		}
	}

}
