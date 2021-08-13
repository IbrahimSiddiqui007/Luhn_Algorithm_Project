package PROJECT1_Siddiqui;

import java.util.Scanner;

public class PROJECT1_Siddiqui
{
    public static boolean cardCheck(Long CardNo)
    {

        int counterAndIndex = 0;
        // This is the counter for the for loop and it is also the index

        int evenDigits = 0;
        // This gets all of the even digits so that they can be multiplied by 2 and added to sEven

        int oddDigits = 0;
        // This gets all of the odd digits so that they can be multiplied by 2 and added to sOdd

        int sEven = 0;
        // This variable is for the sum of all of the even numbers starting from the right of the credit card number

        int sOdd = 0;
        // This variable is for the sum of all of the odd numbers starting from the right of the credit card number

        int totalSum = 0;

        String strCardNo = CardNo.toString();
        // This converts the Long Variable CardNo into a String

        int clen = strCardNo.length();
        // This variable is for getting the length of the credit card

        for (counterAndIndex = clen - 1; counterAndIndex >= 0; counterAndIndex--)
        {
            if (counterAndIndex % 2 == 0 )
            {
                evenDigits = Integer.parseInt(strCardNo.substring(counterAndIndex, counterAndIndex+1));
                evenDigits = evenDigits* 2;
                if (evenDigits > 9 )
                {
                    evenDigits = (evenDigits % 10) + 1;
                }
                sEven += evenDigits;
            }
            else
            {
                oddDigits =  Integer.parseInt(strCardNo.substring(counterAndIndex, counterAndIndex+1));

                sOdd += oddDigits;
            }
        }
        totalSum = sOdd+sEven;

        if (totalSum % 10 == 0)
        {
            return true;
        }
        else
        {

            return false;
        }

    }
    public static void suggestedFix(Long CardNo)
    {
        int counterAndIndex = 0;
        int evenDigits = 0;
        int oddDigits = 0;
        int sEven = 0;
        int sOdd = 0;
        int totalSum = 0;

        String strCardNo = CardNo.toString();
        int clen = strCardNo.length();

        for (counterAndIndex = clen - 1; counterAndIndex >= 0; counterAndIndex--)
        {
            if (counterAndIndex % 2 == 0 )
            {
                evenDigits = Integer.parseInt(strCardNo.substring(counterAndIndex, counterAndIndex+1));
                evenDigits = evenDigits* 2;
                if (evenDigits > 9 )
                {
                    evenDigits = (evenDigits % 10) + 1;
                }
                sEven += evenDigits;
            }
            else
            {
                oddDigits =  Integer.parseInt(strCardNo.substring(counterAndIndex, counterAndIndex+1));
                sOdd += oddDigits;
            }
        }
        totalSum = sOdd+sEven;

        if (CardNo % 10 == 0)
        {
            if (totalSum % 10 >=0  )
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 1)
        {
            if (totalSum % 10 <=8)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=8 && totalSum % 10 <= 9)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 2)
        {
            if (totalSum % 10 <=7)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=7 && totalSum % 10 <= 8)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 3)
        {
            if (totalSum % 10 <=6)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=6 && totalSum % 10 <= 7)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 4)
        {
            if (totalSum % 10 <=5)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=4 && totalSum % 10 <= 5)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 5)
        {
            if (totalSum % 10 <=4)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=4 && totalSum % 10 <= 5)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 6)
        {
            if (totalSum % 10 <= 3)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=3 && totalSum % 10 <= 6)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 7)
        {
            if (totalSum % 10 <=2)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=2 && totalSum % 10 <= 7)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 8)
        {
            if (totalSum % 10 <=1)
            {
                CardNo = CardNo + (totalSum % 10);
                System.out.println(CardNo);
            }
            else if (totalSum % 10 >=1 && totalSum % 10 <= 8)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }
        else if (CardNo % 10 == 9)
        {
            if (totalSum % 10 >=0)
            {
                CardNo = CardNo - (totalSum % 10);
                System.out.println(CardNo);
            }
        }

    }

    public static void main(String[] args)
    {

        Scanner cnInput = new Scanner(System.in);
        // Creating a new scanner. cnInput stands for Credit card number input.

        System.out.println("Please enter the number of Credit Cards: ");
        int amountOfCards = cnInput.nextInt();

        for (int i =0; i < amountOfCards; i++)
        {
            cnInput = new Scanner(System.in);
            // Creating a new scanner. cnInput stands for Credit card number input.

            System.out.println("Please enter your credit card number: ");
            Long CardNo = cnInput.nextLong();
            // This is used to get the credit card number

            String strCardNo = CardNo.toString();
            // This converts the Long Variable CardNo into a String

            if (strCardNo.length() < 17 && strCardNo.length() >= 13)
            {
                if (cardCheck(CardNo) == true && strCardNo.charAt(0) == '4' || strCardNo.charAt(0) == '5' || (strCardNo.charAt(0) == '3'&& strCardNo.charAt(1) == '7') || strCardNo.charAt(0) == '6')
                {
                    if (strCardNo.charAt(0) == '4')
                    {
                        System.out.println("The card: " + strCardNo + " is a Visa Card and it is Valid"  );

                    }
                    else if (strCardNo.charAt(0) == '5')
                    {
                        System.out.println("The card: " + strCardNo + " is a Master Card and it is Valid"  );
                    }
                    else if (strCardNo.charAt(0) == '3'&& strCardNo.charAt(1) == '7')
                    {
                        System.out.println("The card: " + strCardNo + " is an American Express Card and it is Valid"  );
                    }
                    else if (strCardNo.charAt(0) == '6')
                    {
                        System.out.println("The card: " + strCardNo + " is a Discovery Card and it is Valid"  );
                    }

                }
                else if (cardCheck(CardNo) == false && strCardNo.charAt(0) == '4' || strCardNo.charAt(0) == '5' || (strCardNo.charAt(0) == '3'&& strCardNo.charAt(1) == '7') || strCardNo.charAt(0) == '6')
                {
                    if (strCardNo.charAt(0) == '4')
                    {
                        System.out.println("The card: " + strCardNo + " is a Visa Card and it is Invalid"  );
                        System.out.println("The suggested fix for " +strCardNo+ " is ");
                        suggestedFix(CardNo);

                    }
                    else if (strCardNo.charAt(0) == '5')
                    {
                        System.out.println("The card: " + strCardNo + " is a Master Card and it is Invalid"  );
                        System.out.println("The suggested fix for " +strCardNo+ " is");
                        suggestedFix(CardNo);
                    }
                    else if (strCardNo.charAt(0) == '3'&& strCardNo.charAt(1) == '7')
                    {
                        System.out.println("The card: " + strCardNo + " is an American Express Card and it is Invalid"  );
                        System.out.println("The suggested fix for " +strCardNo+ " is");
                        suggestedFix(CardNo);
                    }
                    else if (strCardNo.charAt(0) == '6')
                    {
                        System.out.println("The card: " + strCardNo + " is a Discovery Card and it is Invalid"  );
                        System.out.println("The suggested fix for " +strCardNo+ " is");
                        suggestedFix(CardNo);
                    }
                }
            }
            else
            {
                System.out.println("Sorry this is an invalid card");
            }
        }
    }
}

