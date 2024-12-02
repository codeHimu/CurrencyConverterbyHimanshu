# CurrencyConverterbyHimanshu
public class CurrencyConverter {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter Amount in Indian Rupees(INR)");
        int amount = sc.nextInt();
        // System.out.println("Amount is = "+amount);
        System.out.println("Convert it to Currency:");
        System.out.println("1)  dollar\n" +
                "2)  Euro\n" +
                "3) Kuwaiti Dinar\n"+
                "4) British Pound\n"+
                "5) Swiss Franc"

        );
        int choice = sc.nextInt();
        DecimalFormat df = new DecimalFormat("0.##");
        switch (choice) {
            case 1:
                System.out.println(amount + " INR to Dollar is = " + (df.format(amount / 84.57)));
                System.out.println(amount + " Dollar to INR is = " + (amount * 84.58));
                break;
            case 2:
                System.out.println(amount + " INR to Euro is " + (df.format(+amount / 89.49)));
                System.out.println(amount + " Euro to INR is =" + (amount * 89.49));
                break;
            case 3:
                System.out.println(amount + " INR to Dinar is =" + (df.format(amount / 275.08)));
                System.out.println(amount + " Dinar to INR is =" + amount * 275.08);
            case 4:
                System.out.println(amount +" INR to British Pound is "+(df.format(amount/107.46)));
                System.out.println(amount +" British Pound to INR is "+amount*107.46);
                break;
            case 5:
                System.out.println(amount +" INR to Swiss Franc is "+(df.format(amount/95.78)));
                System.out.println(amount +" Swiss Franc to INR is "+amount*95.78);
                break;
        }
    }
}
