# Assignment--Creditor
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
                Scanner scan = new Scanner(System.in);
        System.out.println("Welcome To ACT Credit Bank");
        System.out.println("We are processing your request for loan");
        System.out.println("Please Enter Your Full Name");
        String name = scan.nextLine();
        System.out.println("Do you have an account no.? Press 1 for YES Press 2 for NO");
        byte acctNo;
        acctNo = scan.nextByte();
        if (acctNo == 1) {
            System.out.println("Has it been six months since you opened your account? Press 1 for YES Press 2 for NO  ");
            byte timeRange;
            timeRange = scan.nextByte();
            if (timeRange == 1) {
                System.out.println("Our bank will lend you 3 times of your Current Balance");
                System.out.println("We have four packages for your repayment");
                System.out.println("Press 1 To pay in 1 year at 5% interest per year");
                System.out.println("Press 2 To pay in 5 year at 10% interest per year");
                System.out.println("Press 3 To pay in 10 year at 15% interest per year");
                System.out.println("Press 4 To pay in 15 year at 20% interest per year");
                int interest, loan;
                interest = scan.nextInt();
                if (interest == 1) {
                    System.out.println("Please Insert Your Currrent Balance");
                    loan = scan.nextInt();
                    System.out.println(("ACT BANK will lend you  ") + (loan * 3));
                    System.out.println(("You will pay  ") + ((loan * 3) + (loan * 3 * 0.05)) + ("  in 1 year"));
                    System.out.println("Press 1 if you agree Press 2 to Exit");
                } else if (interest == 2) {
                    System.out.println("Please Insert Your Currrent Balance");
                    loan = scan.nextInt();
                    System.out.println(("ACT BANK will lend you  ") + (loan * 3));
                    System.out.println(("You will pay  ") + ((loan * 3) + ((loan * 3 * 0.1) * 2)) + ("  in 5 years"));
                    System.out.println("Press 1 if you agree Press 2 to Exit");

                } else if (interest == 3) {
                    System.out.println("Please Insert Your Currrent Balance");
                    loan = scan.nextInt();
                    System.out.println(("ACT BANK will lend you  ") + (loan * 3));
                    System.out.println(("You will pay  ") + ((loan * 3) + ((loan * 3 * 0.15) * 3)) + ("  in 10 years"));
                    System.out.println("Press 1 if you agree Press 2 to Exit");
                } else if (interest == 4) {
                    System.out.println("Please Insert Your Currrent Balance");
                    loan = scan.nextInt();
                    System.out.println(("ACT BANK will lend you  ") + (loan * 3));
                    System.out.println(("You will pay  ") + ((loan * 3) + ((loan * 3 * 0.2) * 4)) + ("  in 15 year"));
                    System.out.println("Press 1 if you agree Press 2 to Exit");}}
            byte agree;
            agree = scan.nextByte();
            if (agree == 1) {
                System.out.println("Do you have a collateral for the loan? Press 1 for Yes Press 2 for no");
                byte colla;
                colla = scan.nextByte();
                if (colla == 1) {
                    System.out.println("Specify your collateral.");
                    System.out.println("Press 1 if your collateral is land or house");
                    System.out.println("Press 2 if your collateral is car or motor vehicle");
                    System.out.println("Press 3 if your collateral is business or business share");
                    byte typeColla;
                    typeColla = scan.nextByte();
                    if (typeColla == 1) {
                        System.out.println("Do you have full ownership? Press 1 for Yes Press 2 for No");
                        byte own;
                        own = scan.nextByte();
                        if (own == 1) {
                            System.out.println("You are almost done. One last Question.");
                            System.out.println("Do you have a criminal record? Press 1 for Yes Press 2 for N0");
                        } else
                            System.out.println("Your process has been terminated. Please contact our employees at the front desk");
                    }
                    if (typeColla == 2) {
                        System.out.println("Do you have full ownership? Press 1 for Yes Press 2 for No");
                        byte own;
                        own = scan.nextByte();
                        if (own == 1) {
                            System.out.println("You are almost done. One last Question.");
                            System.out.println("Do you have a criminal record? Press 1 for Yes Press 2 for N0");
                        } else
                            System.out.println("Your process has been terminated. Please contact our employees at the front desk");

                    }
                    if (typeColla == 3) {
                        System.out.println("Do you have full ownership? Press 1 for Yes Press 2 for No");
                        byte own;
                        own = scan.nextByte();
                        if (own == 1) {
                            System.out.println("You are almost done. One last Question.");
                            System.out.println("Do you have a criminal record? Press 1 for Yes Press 2 for N0");
                        } else
                            System.out.println("Your process has been terminated. Please contact our employees at the front desk");
                    }}
                byte criminal;
                criminal = scan.nextByte();
                if (criminal == 2) {
                            System.out.println("Congrtulation your loan has been approved.");
                            System.out.println("Please contact our employees at the front desk");
                            System.out.println("Thank You for choosing ACT BANK ");
                        } else System.out.println("Your process has been terminated. Please contact our employees at the front desk");


                    } else System.out.println("Your process has been terminated. Please contact our employees at the front desk");


                } else System.out.println("Your process has been terminated. Please contact our employees at the front desk");


    }
}
