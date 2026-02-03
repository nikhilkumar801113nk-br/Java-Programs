import java.util.*;
public class linearsearch {
    public static int linearsearch(int number[], int key) {
        for (int i = 0; i < number.length; i++) {
            if (number[i] == key) {
                return i; // return index immediately
            }
        }
        return -1; // if key not found
    }

    public static void main(String args[]) {
        int number[] = {1, 2, 3, 8, 6, 7, 9};
        int key = 8;

        int index = linearsearch(number, key);

        if (index == -1) {
            System.out.println("not found");
        } else {
            System.out.println("found at index: " + index);
        }
    }
}
