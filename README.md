# Assignment-No-5
Assignment no 5


Assignment No 5 ////////////////////////





public class FindMissingNumber {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 4, 5, 6};
        int missing = findMissing(numbers);
        System.out.println("The missing number is: " + missing);
    }

    public static int findMissing(int[] numbers) {
        int n = numbers.length + 1;
        int totalSum = n * (n + 1) / 2;
        int sum = 0;

        for (int num : numbers) {
            sum += num;
        }

        return totalSum - sum;
    }
}
