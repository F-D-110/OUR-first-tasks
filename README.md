# OUR-first-tasks

import java.util.Stack;

public class ArrayReversal {
    public static void reverseArray(int[] array) {
        Stack<Integer> stack = new Stack<>();

        // Push elements onto the stack
        for (int element : array) {
            stack.push(element);
        }

        // Pop elements from the stack and store them back in the array
        for (int i = 0; i < array.length; i++) {
            array[i] = stack.pop();
        }
    }

    public static void main(String[] args) {
        int[] array = {1, 2, 3, 4, 5};
        System.out.println("Original Array:");
        for (int element : array) {
            System.out.print(element + " ");
        }

        reverseArray(array);

        System.out.println("\nReversed Array:");
        for (int element : array) {
            System.out.print(element + " ");
        }
    }
}
