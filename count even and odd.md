public class count {
    public static int evenOdd(int number) {
        int evenCount = 0;
        int oddCount = 0;

        while(number > 0) {
            int digit = number % 10;
              if(digit % 10 == 0) {
                evenCount++;
              } else {
              oddCount++;
              }
              number = number /10;
        }  
        return evenCount + oddCount;
        
    }

    public static void main(String args[]) {
               System.out.println(evenOdd(123456789));
    }
}
