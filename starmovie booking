import java.sql.SQLOutput;
import java.time.format.DateTimeFormatter;
import java.util.Date;
import java.util.InputMismatchException;
import java.util.Random;
import java.util.Scanner;
import java.time.*;

public class starmovieBooking {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        try {
            System.out.print("LOADING");
            for (int g = 0; g <= 3; g++) {
                Thread.sleep(500);
                System.out.print(".");
            }
        } catch(InterruptedException e) {
            System.out.println("INTERRUPTED ERROR");
        }



            System.out.println("\n                   WELCOME TO STARMOVIE!");
            System.out.println("           Book your movies with cozy rooms here!");
            System.out.println("\n|        ROOM         |    RATES    |      CAPACITY      |");
            System.out.println("----------------------------------------------------------");
            System.out.println("| 1. Couple Room      |  ₱125/head  |  Up to 2 persons   |");
            System.out.println("| 2. Family Room      |  ₱100/head  |  Up to 5 persons   |");
            System.out.println("| 3. Barkadahan Room  |  ₱75/head   |  Up to 10 persons  |");
            //creates a loop if conditions met is true
            while (true) {
                System.out.println("\nWould you like to book your reservations today?");
                String answer = sc.nextLine().toLowerCase();
                if (answer.matches(".*\\d.*")) {
                    //checks if input has numbers in it and generates error if it has
                    System.out.println("ERROR: Characters should not contain numbers, (y/n) only!");
                } else if (answer.equals("n")) {
                    System.out.println("Thank you for visiting Starmovie! Have a great day!");
                    System.exit(0);
                } else if (answer.equals("y")) {
                    break;
                    //if answer is y or no, breaks out of the loop
                } else {
                    System.out.println("ERROR: Only accepts answers - (y/n)!");
                }
            }
            //body outside while loop
            try {
                // code that uses Thread.sleep() goes here
                System.out.print("Loading");

                for (int i = 0; i < 3; i++) {
                    Thread.sleep(500); // pause for half a second
                    System.out.print(".");
                }

                System.out.println();
            } catch (InterruptedException e) {
                // handle the exception here
                System.out.println("ERROR");

            }
            String customerName = "";
            while (true) {
                System.out.println("\nEnter Customer Name: ");
                customerName = sc.nextLine();
                if (customerName.matches(".*\\d.*")) {
                    System.out.println("ERROR: Customer name should not have numerical characters!");
                } else {
                    break;
                }
            }
            //body outside of loop
            while (true) {
                System.out.println("Enter Customer Age:");
                try {
                    int customerAge = sc.nextInt();
                    if (customerAge < 18) {
                        System.out.println("Minors are not allowed!");
                    } else {
                        break;
                    }
                } catch (InputMismatchException e) {
                    System.out.println("ERROR: Customer age should not have alphabetical characters!");
                    sc.nextLine();
                }
            }
            System.out.println("\n|----GENRE LIST----|");
            System.out.println("|    1. Cartoon    |");
            System.out.println("|    2. Comedy     |");
            System.out.println("|    3. Horror     |");
            System.out.println("|    4. Love Story |");
            System.out.println("|------------------|");
            String genre, movie;
            genre = "";
            movie = "";
            boolean boolMovie = false; //create boolean variable that indicates false
            boolean boolGenre = false;

            while (!boolGenre) {
                System.out.println("Select Genre (1-4):");
                try {
                    int customerGenre = sc.nextInt();
                    if (customerGenre >= 1 && customerGenre <= 4) {
                        boolGenre = true;
                        switch (customerGenre) {
                            case 1:
                                System.out.println("\n|------------CARTOON MOVIE LIST-------------|");
                                System.out.println("|         Movie Title          |  Duration  |");
                                System.out.println("|-------------------------------------------|");
                                System.out.println("| 1. Kung fu Panda             |  1:32:00   |");
                                System.out.println("| 2. Wendell & Wild            |  1:45:00   |");
                                System.out.println("| 3. The Grinch                |  1:30:00   |");
                                System.out.println("| 4. The Lion King             |  1:29:00   |");
                                System.out.println("| 5. Toy Story                 |  1:21:00   |");
                                System.out.println("|-------------------------------------------|");
                                genre = "CARTOON";
                                // while the statement is false, this body of code will loop
                                while (!boolMovie) {
                                    System.out.println("Select Movie (1-5):");
                                    try {
                                        int customerMovie = sc.nextInt();
                                        if (customerMovie >= 1 && customerMovie <= 5) {
                                            boolMovie = true;
                                            // if number inputted is between 1-5 which are valid numbers, end loop

                                            switch (customerMovie) {
                                                case 1:
                                                    movie = "Kung fu Panda";
                                                    break;
                                                case 2:
                                                    movie = "Wendell & Wild";
                                                    break;
                                                case 3:
                                                    movie = "The Grinch";
                                                    break;
                                                case 4:
                                                    movie = "The Lion King";
                                                    break;
                                                case 5:
                                                    movie = "Toy Story";
                                                    break;
                                            }
                                        } else {
                                            System.out.println("ERROR: Movie selection is 1-5 only!");
                                        }
                                    } catch (InputMismatchException e) {
                                        System.out.println("ERROR: Movie selection should not have alphabetical characters!");
                                        sc.nextLine();
                                    }
                                }

                                break;
                            case 2:
                                System.out.println("\n|------------COMEDY MOVIE LIST-------------|");
                                System.out.println("|         Movie Title          |  Duration  |");
                                System.out.println("|-------------------------------------------|");
                                System.out.println("| 1. Bullet Train              |  1:29:00   |");
                                System.out.println("| 2. Lyle,Lyle Crocodile       |  2:10:00   |");
                                System.out.println("| 3. Me Time                   |  1:56:00   |");
                                System.out.println("| 4. Easter Sunday             |  1:58:00   |");
                                System.out.println("| 5. Junex                     |  1:49:00   |");
                                System.out.println("|-------------------------------------------|");
                                genre = "COMEDY";
                                while (!boolMovie) {
                                    System.out.println("Select Movie (1-5):");
                                    try {
                                        int customerMovie = sc.nextInt();
                                        if (customerMovie >= 1 && customerMovie <= 5) {
                                            boolMovie = true;
                                            // if number inputted is between 1-5 which are valid numbers, end loop

                                            switch (customerMovie) {
                                                case 1:
                                                    movie = "Bullet Train";
                                                    break;
                                                case 2:
                                                    movie = "Lyle,Lyle Crocodile";
                                                    break;
                                                case 3:
                                                    movie = "Me Time";
                                                    break;
                                                case 4:
                                                    movie = "Easter Sunday";
                                                    break;
                                                case 5:
                                                    movie = "Junex";
                                                    break;
                                            }
                                        } else {
                                            System.out.println("ERROR: Movie selection is 1-5 only!");
                                        }
                                    } catch (InputMismatchException e) {
                                        System.out.println("ERROR: Movie selection should not have alphabetical characters!");
                                        sc.nextLine();
                                    }
                                }

                                break;
                            case 3:
                                System.out.println("\n|------------HORROR MOVIE LIST--------------|");
                                System.out.println("|         Movie Title          |  Duration  |");
                                System.out.println("|-------------------------------------------|");
                                System.out.println("| 1. IT                        |  2:15:00   |");
                                System.out.println("| 2. Hereditary                |  2:07:00   |");
                                System.out.println("| 3. A Quiet Place             |  1:30:00   |");
                                System.out.println("| 4. The Menu                  |  1:47:00   |");
                                System.out.println("| 5. The Exorcist              |  2:12:00   |");
                                System.out.println("|-------------------------------------------|");
                                genre = "HORROR";
                                while (!boolMovie) {
                                    System.out.println("Select Movie (1-5):");
                                    try {
                                        int customerMovie = sc.nextInt();
                                        if (customerMovie >= 1 && customerMovie <= 5) {
                                            boolMovie = true;
                                            // if number inputted is between 1-5 which are valid numbers, end loop

                                            switch (customerMovie) {
                                                case 1:
                                                    movie = "IT";
                                                    break;
                                                case 2:
                                                    movie = "Hereditary";
                                                    break;
                                                case 3:
                                                    movie = "A Quiet Place";
                                                    break;
                                                case 4:
                                                    movie = "The Menu";
                                                    break;
                                                case 5:
                                                    movie = "The Exorcist";
                                                    break;
                                            }
                                        } else {
                                            System.out.println("ERROR: Movie selection is 1-5 only!");
                                        }
                                    } catch (InputMismatchException e) {
                                        System.out.println("ERROR: Movie selection should not have alphabetical characters!");
                                        sc.nextLine();
                                    }
                                }

                                break;
                            case 4:
                                System.out.println("\n|------------LOVE STORY MOVIE LIST--------------|");
                                System.out.println("|  Movie Title                 |  Duration  |");
                                System.out.println("|-------------------------------------------|");
                                System.out.println("| 1. Goblin                    |  1:45:00   |");
                                System.out.println("| 2. Be careful with my heart  |  1:33:00   |");
                                System.out.println("| 3. Meteor garden             |  1:33:00   |");
                                System.out.println("| 4. True beauty               |  1:32:00   |");
                                System.out.println("| 5. I am not a robot          |  1:45:00   |");
                                System.out.println("|-------------------------------------------|");
                                genre = "LOVE STORY";
                                while (!boolMovie) {
                                    System.out.println("Select Movie (1-5):");
                                    try {
                                        int customerMovie = sc.nextInt();
                                        if (customerMovie >= 1 && customerMovie <= 5) {
                                            boolMovie = true;
                                            // if number inputted is between 1-5 which are valid numbers, end loop

                                            switch (customerMovie) {
                                                case 1:
                                                    movie = "Goblin";
                                                    break;
                                                case 2:
                                                    movie = "Be careful with my heart";
                                                    break;
                                                case 3:
                                                    movie = "Meteor garden";
                                                    break;
                                                case 4:
                                                    movie = "True beauty";
                                                    break;
                                                case 5:
                                                    movie = "I am not a robot";
                                                    break;
                                            }
                                        } else {
                                            System.out.println("ERROR: Movie selection is 1-5 only!");
                                        }
                                    } catch (InputMismatchException e) {
                                        System.out.println("ERROR: Movie selection should not have alphabetical characters!");
                                        sc.nextLine();
                                    }
                                }

                                break;
                        }
                    } else {
                        System.out.println("ERROR: Genre selection is 1-4 only!");
                    }

                } catch (InputMismatchException e) {
                    System.out.println("ERROR: Genre selection should not have alphabetical characters!");
                    sc.nextLine();
                }
            }

            DateTimeFormatter dateFormat = DateTimeFormatter.ofPattern("E,MMM dd yyyy"); // format for date to display
            LocalDate dateToday = LocalDate.now(); // get current date and store to variable
            LocalDate date1 = dateToday.plusDays(1); // create dates after current date (plusDays)
            LocalDate date2 = dateToday.plusDays(2);
            LocalDate date3 = dateToday.plusDays(3);
            LocalDate date4 = dateToday.plusDays(4);
            LocalDate date5 = dateToday.plusDays(5);

            System.out.println("\nAvailable Dates of Reservation");
            System.out.println("1. " + date1.format(dateFormat));
            System.out.println("2. " + date2.format(dateFormat));
            System.out.println("3. " + date3.format(dateFormat));
            System.out.println("4. " + date4.format(dateFormat));
            System.out.println("5. " + date5.format(dateFormat));

            boolean boolReserDate = false;
            String reservationDate = "";
            while (!boolReserDate) {
                System.out.println("\nSelect Date (1-5): ");
                try {
                    int reservationDateInput = sc.nextInt();
                    if (reservationDateInput >= 1 && reservationDateInput <= 5) {
                        boolReserDate = true;
                        switch (reservationDateInput) {
                            case 1:
                                reservationDate = date1.format(dateFormat);
                                break;
                            case 2:
                                reservationDate = date2.format(dateFormat);
                                break;
                            case 3:
                                reservationDate = date3.format(dateFormat);
                                break;
                            case 4:
                                reservationDate = date4.format(dateFormat);
                                break;
                            case 5:
                                reservationDate = date5.format(dateFormat);
                                break;
                        }
                    } else {
                        System.out.println("ERROR: Reservation Date Selection is 1-5 only!");
                        boolReserDate = false;
                    }
                } catch (InputMismatchException e) {
                    System.out.println("ERROR: Date selection should not have alphabetical characters!");
                    sc.nextLine();
                }
            }
            boolean boolCustomerQuantity = false;
            int roomPerHead = 0;
            int totalAmount = 0;
            String roomType = "";
            while (!boolCustomerQuantity) {
                System.out.println("\nEnter Number of Customers:");
                try {
                    int customerQuantity = sc.nextInt();
                    if (customerQuantity > 10 || customerQuantity < 1) {
                        System.out.println("Only up to 10 persons are allowed each room");
                    } else if (customerQuantity <= 2) {
                        System.out.println("Available Room: Couple Room --> ₱125/head");
                        roomPerHead = 125;
                        roomType = "Couple Room";
                        totalAmount = customerQuantity * roomPerHead;
                        boolCustomerQuantity = true;
                    } else if (customerQuantity <= 5) {
                        System.out.println("Available Room: Family Room --> ₱100/head");
                        roomPerHead = 100;
                        roomType = "Family Room";
                        totalAmount = customerQuantity * roomPerHead;
                        boolCustomerQuantity = true;
                    } else {
                        System.out.println("Available Room: Barkadahan Room --> ₱75/head");
                        roomPerHead = 75;
                        roomType = "Barkadahan Room";
                        totalAmount = customerQuantity * roomPerHead;
                        boolCustomerQuantity = true;
                    }
                } catch (InputMismatchException e) {
                    System.out.println("ERROR: Customer Quantity should not have alphabetical letters!");
                    sc.nextLine();
                }
            }
            double totalAmountMoney = totalAmount;
            System.out.println("TOTAL AMOUNT: ₱ " + totalAmountMoney);

            boolean boolMoneyInput = false;
            double customerMoney, customerChange;
            customerMoney = 0;
            customerChange = 0;
            while (!boolMoneyInput) {
                System.out.println("\nEnter Money:");
                try {
                    customerMoney = sc.nextInt();
                    if (customerMoney < totalAmountMoney) {
                        System.out.println("ERROR: Money is Insufficient!");
                    } else {
                        customerChange = customerMoney - totalAmountMoney;
                        System.out.println("Change: ₱ " + customerChange);
                        boolMoneyInput = true;
                    }
                } catch (InputMismatchException e) {
                    System.out.println("ERROR: Money Input should not have alphabetical letters!");
                    sc.nextLine();
                }
            }

            try {
                System.out.print("\nGenerating Receipt");
                for (int j = 0; j < 5; j++) {
                    Thread.sleep(500);
                    System.out.print(".");
                }
                System.out.println();
            } catch (InterruptedException e) {
                System.out.println("ERROR");
            }

            Random random = new Random();
            int customerCode = random.nextInt(99999999 - 10000000) + 10000000;
            LocalTime timeToday = LocalTime.now();
            DateTimeFormatter receiptReservationDateFormat = DateTimeFormatter.ofPattern("E, MMM dd yyyy");
            DateTimeFormatter receiptDateFormat = DateTimeFormatter.ofPattern("dd-MM-yyyy");
            DateTimeFormatter receiptTimeFormat = DateTimeFormatter.ofPattern("HH:mm:ss");

            System.out.println();
            System.out.println("--------------------------------------------------------");
            System.out.println("              STARMOVIE RESERVATION RECEIPT             ");
            System.out.println("                     " + dateToday.format(receiptDateFormat));
            System.out.println("                      " + timeToday.format(receiptTimeFormat));
            System.out.println();
            System.out.println("  Reservant Name: " + customerName.toUpperCase());
            System.out.println("  Date of Booking: " + dateToday.format(receiptReservationDateFormat));
            System.out.println("  Date of Reservation: " + reservationDate);
            System.out.println("  Movie: " + movie.toUpperCase());
            System.out.println("  Room: " + roomType.toUpperCase());
            System.out.println("  Code: " + customerCode);
            System.out.println("--------------------------------------------------------");


    }
}


