# warm-up-for-ds
warming up
public class MyFirstHomeworkFor300{

    public static double minValue(double[] list) {

        double min = list[0];

        for (int i = 1; i < list.length; i++) {

            if (list[i] < min) {

                min = list[i];

            }

        }

        return min;

    }

    public static int minPosition(double[] list) {

        int minIndex = 0;

        double min = list[0];

        for (int i = 1; i < list.length; i++) {

            if (list[i] < min) {

                min = list[i];

                minIndex = i;

            }

        }

        return minIndex;

    }
public static int distanceBetweenMinAndMax(double[] list) {

        int minIndex = 0, maxIndex = 0;

        double min = list[0], max = list[0];

        for (int i = 1; i < list.length; i++) {

            if (list[i] < min) {

                min = list[i];

                minIndex = i;

            }

            if (list[i] > max) {

                max = list[i];

                maxIndex = i;

            }

        }

        return Math.abs(maxIndex - minIndex);

    }

    public static void main(String[] args) {

        double[] list = {1, -4, -7, 7, 8, 11};

        System.out.println("minValue: " + minValue(list)); // Expected: -7

        System.out.println("minPosition: " + minPosition(list)); // Expected: 2

        System.out.println("distanceBetweenMinAndMax: " + distanceBetweenMinAndMax(list)); // Expected: 3

    }

}    
