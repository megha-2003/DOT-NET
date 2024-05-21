9.1 ADMIN BLOCK 
 
    List<int> a9 = new List<int>(); 
    Console.ForegroundColor = ConsoleColor.Yellow; 
    Console.WriteLine("-------------------WELCOME TO ONLINE SHOPPING--------------------"); 
    Console.WriteLine(); 
    Console.ForegroundColor = ConsoleColor.Magenta; 
Y: Console.WriteLine("               Choose the Login type"); 
    Console.WriteLine("                   1. ADMIN"); 
    Console.WriteLine("                   2. USER"); 
    a = Convert.ToInt32(Console.ReadLine()); 
    Console.Clear(); 
    if (a == 1) 
    { 
        Console.ForegroundColor = ConsoleColor.Green; 
        Console.WriteLine("              WELCOME TO ADMIN PAGE     "); 
        Console.WriteLine(); 
        Console.ForegroundColor = ConsoleColor.Red; 
        Console.WriteLine("              ADMIN Login ID : ADMIN"); 
        Console.WriteLine("              ADMIN Password : ADMIN"); 
        Console.WriteLine(); 
        Console.ForegroundColor = ConsoleColor.Cyan; 
        Console.WriteLine("         Do you want to reset Admin password"); 
        Console.WriteLine("                1. Yes"); 
        Console.WriteLine("                2. No"); 
        a2 = Convert.ToInt32(Console.ReadLine()); 
        Console.Clear(); 
        if (a2 == 1) 
        { 
            Console.WriteLine(); 
            Console.ForegroundColor = ConsoleColor.Blue; 
        B: Console.Write("Enter you New password (8 characters Only) : "); 
            a3 = Console.ReadLine(); 
            Console.Clear(); 
            if (a3.Length > 8) 
            { 
                Console.WriteLine(); 
                Console.ForegroundColor = ConsoleColor.Red; 
                Console.WriteLine("Entered password is not in specified format!Please try again "); 
                Console.Clear(); 
                goto B; 
                         
            } 
            else 
            { 
                Console.WriteLine("Admin Password updated Successfully.."); 
(11) 
                a1 = a3; 
            } 
            Console.WriteLine(); 
            Console.ForegroundColor = ConsoleColor.Red; 
            Console.WriteLine("             WELCOME TO LOGIN PAGE"); 
            Console.ForegroundColor = ConsoleColor.Green; 
            Console.WriteLine(); 
        C: Console.WriteLine("              ADMIN Login ID : ADMIN"); 
            Console.Write("              ADMIN Password : "); 
            a4 = Console.ReadLine(); 
            Console.Clear(); 
            if (a4 == a1) 
            { 
                Console.WriteLine(); 
                Console.ForegroundColor = ConsoleColor.Red; 
                Console.WriteLine("         WELCOME TO ADMIN DASHBOARD"); 
            } 
            else 
            { 
                Console.WriteLine("Password is Incoorect!Please tryagain"); 
                goto C; 
            } 
            Console.WriteLine(); 
            Console.ForegroundColor = ConsoleColor.Green; 
            Console.WriteLine("           Do You want to add items"); 
            Console.WriteLine("                1. Yes"); 
            Console.WriteLine("                2. No"); 
            a5 = Convert.ToInt32(Console.ReadLine()); 
            Console.Clear(); 
            if (a5 == 1) 
            { 
                Console.WriteLine(); 
 
                Console.ForegroundColor = ConsoleColor.Green; 
                Console.WriteLine("Enter number of items to be added"); 
                b = Convert.ToInt32(Console.ReadLine()); 
                Console.Clear(); 
                for (int i = 1; i <= b; i++) 
                { 
                    Console.WriteLine(); 
                    Console.ForegroundColor = ConsoleColor.DarkCyan; 
                    Console.WriteLine("Enter the name of the " + i + " item"); 
                    d3[i] = Console.ReadLine(); 
                    Console.WriteLine("Enter the Cost of the " + i + " item"); 
                    d4[i] = Convert.ToInt32(Console.ReadLine()); 
                } 
                Console.Clear(); 
                Console.WriteLine(); 
                Console.ForegroundColor = ConsoleColor.Magenta; 
                Console.WriteLine("Name of the item" + "             " + "Cost of the item"); 
(12) 
                for (int i = 1; i <= b; i++) 
                { 
                    Console.WriteLine("    " + d3[i] + "                      " + d4[i]); 
 
                } 
                         
 
 
 
                goto Y; 
            } 
 
        }  
(13) 
 
 
 
9.2 USER BLOCK 
 
    if(a2==2) 
    { 
        Console.WriteLine("WELCOME TO ADMIN LOGIN"); 
        Console.WriteLine("ADMIN LOGIN:ADMIN"); 
            Console . WriteLine("ADMIN PASSWORD:ADMIN"); 
        Console.WriteLine("           Do You want to add items"); 
        Console.WriteLine("                1. Yes"); 
        Console.WriteLine("                2. No"); 
        a5 = Convert.ToInt32(Console.ReadLine()); 
        Console.Clear(); 
        if (a5 == 1) 
        { 
            Console.WriteLine(); 
 
            Console.ForegroundColor = ConsoleColor.Green; 
            Console.WriteLine("Enter number of items to be added"); 
            b = Convert.ToInt32(Console.ReadLine()); 
            for (int i = 1; i <= b; i++) 
            { 
                Console.WriteLine(); 
                Console.ForegroundColor = ConsoleColor.DarkCyan; 
                Console.WriteLine("Enter the name of the " + i + " item"); 
                d3[i] = Console.ReadLine(); 
                Console.WriteLine("Enter the Cost of the " + i + " item"); 
                d4[i] = Convert.ToInt32(Console.ReadLine()); 
            } 
            Console.Clear(); 
            Console.WriteLine(); 
            Console.ForegroundColor = ConsoleColor.Magenta; 
            Console.WriteLine("Name of the item" + "             " + "Cost of the item"); 
            for (int i = 1; i <= b; i++) 
            { 
                Console.WriteLine("    " + d3[i] + "                      " + d4[i]); 
 
            } 
             
 
 
            goto Y; 
        } 
 
    } 
} 
if (a == 2) 
{ 
(14) 
    Console.WriteLine("Name of the item" + "                 " + "Cost of the item"); 
    Console.ForegroundColor = ConsoleColor.DarkGray; 
 
    for (int i = 1; i <= b; i++) 
    { 
        Console.WriteLine("    " + d3[i] + "                      " + d4[i]); 
 
    } 
    Console.WriteLine("Enter how many items you neeed to add in your cart"); 
    a12 = Convert.ToInt32(Console.ReadLine()); 
    if (a12 != 0) 
    { 
        int[] a16 = new int[a12]; 
        for (int i = 0; a16.Length > i; i++) 
        { 
            Console.WriteLine("please enter the number you want to add the item in your 
cart(index number):"); 
            a16[i] = Convert.ToInt32(Console.ReadLine()); 
            Console.WriteLine("Enter how many units you need"); 
            a14 = Convert.ToInt32(Console.ReadLine()); 
            a9.Add(a14); 
        } 
        Console.Clear(); 
        Console.WriteLine("CART"); 
        Console.WriteLine("NAME OF THE ITEM" + "                        " + "UNITS" + "                            
" + "COST OF THE ITEM"); 
        for (int i = 0; a16.Length > i; i++) 
        { 
            Console.WriteLine(d3[a16[i]] + "                           " + a9[i] + "                                              
" + d4[a16[i]]); 
        } 
        O: Console.WriteLine("Do You want to continue shopping"); 
        Console.WriteLine("1.Yes"); 
        Console.WriteLine("2.No"); 
        a12 = Convert.ToInt32(Console.ReadLine()); 
        if (a12 == 1) 
        { 
            Console.WriteLine("Name of the item" + "                 " + "Cost of the item"); 
            Console.ForegroundColor = ConsoleColor.DarkGray; 
 
            for (int i = 1; i <= b; i++) 
            { 
                Console.WriteLine("    " + d3[i] + "                      " + d4[i]); 
 
            } 
            Console.WriteLine("Enter number of items to be added"); 
            a20=Convert.ToInt32(Console.ReadLine()); 
             int[] c10 = new int[a20]; 
            for(int i=0;c10.Length>i;i++) 
            { 
(15) 
                Console.WriteLine("please enter the number you want to add the item in your 
cart:"); 
                a16[i] = Convert.ToInt32(Console.ReadLine()); 
                Console.WriteLine("Enter how many units you need"); 
                a14 = Convert.ToInt32(Console.ReadLine()); 
                a9.Add(a14); 
            } 
            Console.WriteLine("NAME OF THE ITEM" + "                        " + "UNITS" + "                            
" + "COST OF THE ITEM"); 
            for (int i = 0; c10.Length > i; i++) 
            { 
                Console.WriteLine(d3[c10[i]] + "                 " + a9[i] + "                          " + 
d4[c10[i]]); 
            } 
 
            Console.Clear(); 
 
            Console.ForegroundColor = ConsoleColor.DarkCyan; 
            for (int i = 0; c10.Length > i; i++) 
            { 
                int m, o; 
                string n; 
                m = d4[a16[i]]; 
                n = d3[a16[i]]; 
                o = a9[i]; 
                total1 = total1 + (m * o); 
 
                Console.WriteLine(n + "                                 " + o + "                               " + m); 
            } 
 
 
            double gsta; 
            gsta = (total1 * 18) / 100; 
            gst1= total1 + gsta; 
 
            goto O; 
 
        } 
        if (a12 == 2) 
        { 
            Console.WriteLine("Are you ready for billing"); 
            Console.WriteLine("1.Yes"); 
            Console.WriteLine("2.No"); 
            a10 = Convert.ToInt32(Console.ReadLine()); 
            Console.Clear(); 
            if (a10 == 1) 
            { 
                string name, email, str, lan, ci, st, cu, us, p, mob, u1, p1; 
                int pin; 
                Console.WriteLine(); 
(16) 
                Console.ForegroundColor = ConsoleColor.DarkGreen; 
                Console.Write("Name      :"); 
                Console.WriteLine(); 
                name = Console.ReadLine(); 
            V: Console.Write("Contact no :"); 
                Console.WriteLine(); 
                mob = Console.ReadLine(); 
                Regex x = new Regex(pattern); 
                Console.ForegroundColor = ConsoleColor.Red; 
                if (x.IsMatch(mob.ToString())) 
                { 
                    Console.WriteLine("String matched"); 
                } 
                else 
                { 
                    Console.WriteLine("String not matched"); 
                    goto V; 
 
                } 
                Console.ForegroundColor = ConsoleColor.DarkGreen; 
                Console.WriteLine(); 
            N1: Console.Write("Mail Id   : "); 
 
                email = Console.ReadLine(); 
                Regex x1 = new Regex(pattern1); 
                Console.ForegroundColor = ConsoleColor.Red; 
                if (x1.IsMatch(email)) 
                { 
                    Console.WriteLine(); 
                    Console.WriteLine("Entered email is in correct format"); 
                } 
                else 
                { 
                    Console.WriteLine("Entered Email is not in Correct format!Please try again"); 
                    goto N1; 
                } 
                Console.ForegroundColor = ConsoleColor.DarkGreen; 
                Console.WriteLine(); 
                Console.WriteLine("Address:"); 
                Console.WriteLine(); 
                Console.Write("Street name :"); 
                str = Console.ReadLine(); 
                Console.WriteLine(); 
                Console.Write("Land mark :"); 
                lan = Console.ReadLine(); 
                Console.WriteLine(); 
                Console.Write("City      :"); 
                ci = Console.ReadLine(); 
                Console.WriteLine(); 
            N4: Console.Write("Pincode   :"); 
(17) 
                pin = Convert.ToInt32(Console.ReadLine()); 
                Console.WriteLine(); 
                Console.ForegroundColor = ConsoleColor.Red; 
                if (pin.ToString().Length > 7) 
                { 
                    Console.WriteLine("Enter the pin code correctly..."); 
                    goto N4; 
                } 
                Console.ForegroundColor = ConsoleColor.DarkGreen; 
 
                Console.Write("State    :"); 
                st = Console.ReadLine(); 
                Console.Write("Country  : "); 
                cu = Console.ReadLine(); 
            N2: Console.Write("User Id  :"); 
                us = Console.ReadLine(); 
                Console.ForegroundColor = ConsoleColor.Red; 
                if (us.Length > 9) 
                { 
                    Console.WriteLine("Please Specify Only 8 characters"); 
                    goto N2; 
 
                } 
                Console.ForegroundColor = ConsoleColor.DarkGreen; 
            N3: Console.Write("User Password :"); 
                p = Console.ReadLine(); 
                Console.ForegroundColor = ConsoleColor.Red; 
                if (p.Length > 8) 
                { 
                    Console.WriteLine("Enter password in specified format"); 
                    goto N3; 
                } 
 
 
                Console.Clear(); 
                Console.ForegroundColor = ConsoleColor.Magenta; 
                Console.WriteLine("WELCOME TO USER LOGIN FORM"); 
                Console.Write("USER ID         : "); 
                u1 = Console.ReadLine(); 
                Console.WriteLine("PASSWORD    :"); 
                p1 = Console.ReadLine(); 
                Console.ForegroundColor = ConsoleColor.Green; 
                if (u1 == us && p1 == p) 
                { 
                    Console.WriteLine("Logged in Successfully"); 
                    Console.ForegroundColor = ConsoleColor.Magenta; 
                    Console.WriteLine("Name of the item" + "                  " + "Units " + "                           
" + "Cost of the item"); 
                    double total = 0; 
                    Console.ForegroundColor = ConsoleColor.DarkCyan; 
(18) 
                    for (int i = 0; a16.Length > i; i++) 
                    { 
                        int m, o; 
                        string n; 
                        m = d4[a16[i]]; 
                        n = d3[a16[i]]; 
                        o = a9[i]; 
                        total = total + (m * o); 
 
                        Console.WriteLine(n + "                                 " + o + "                               " + 
m); 
                    } 
 
 
                    double gsta, gst; 
                    gsta = (total * 18) / 100; 
                    gst = total + gsta+gst1; 
                    
Console.WriteLine("===================================================
 ==================================================================
 ==========="); 
                    Console.WriteLine(); 
                    Console.ForegroundColor = ConsoleColor.Yellow; 
                    Console.WriteLine("_ BILLING_"); 
                    Console.WriteLine("Name : " + name); 
                    Console.WriteLine("Contact number" + mob); 
                    Console.WriteLine("NAME OF THE ITEM" + "             " + "UNITS" + "                 
" + "COST OF THE ITEM"); 
                    for (int i = 0; a16.Length > i; i++) 
                    { 
                        int m, o; 
                        string n; 
                        m = d4[a16[i]]; 
                        n = d3[a16[i]]; 
                        o = a9[i]; 
 
 
                        Console.WriteLine(n + "                                   " + o + "                               " + 
m); 
                    } 
                    Console.WriteLine("-------------------------------------------------------------------------------------------------------------"); 
                    Console.WriteLine("Total:" + "                               " + total); 
                    Console.WriteLine("--------------------------------------------------------------------------------------------------------------"); 
                    Console.WriteLine("GST: 18%"); 
                    Console.WriteLine("---------------------------------------------------------------------------------------------------------------"); 
                    Console.WriteLine("Total Bill:" + "                            " + gst); 
 
(19) 
                } 
 
            } 
            if(a10==2) 
            { 
                Console.WriteLine(); 
                Console.ForegroundColor = ConsoleColor.Yellow; 
            P: Console.WriteLine("    Do You want to remove any item in the cart"); 
                Console.WriteLine("                  1. Yes"); 
                Console.WriteLine("                  2. No"); 
                a12 = Convert.ToInt32(Console.ReadLine()); 
                if (a12 == 1) 
                { 
                    for (int i = 0; a16.Length > i; i++) 
                    { 
                        Console.WriteLine(d3[a16[i]] + "                                   " + a9[i] + "                                  
" + d4[a16[i]]); 
                    } 
                    Console.WriteLine(); 
                    Console.ForegroundColor = ConsoleColor.Blue; 
                    Console.WriteLine("Enter how many items to be removed"); 
                    a14 = Convert.ToInt32(Console.ReadLine()); 
                    if (a14 >= 0 && a14 < a16.Length) 
                    { 
                        a16 = a16.Where((val, idx) => idx != a14).ToArray(); 
                        a9.RemoveAt(a14); 
                        Console.WriteLine("Item removed from cart Successfully"); 
 
                    } 
                    else 
                    { 
                        Console.WriteLine("Invalid Item Index!Please.Try again"); 
 
                    } 
                    for (int i = 0; a16.Length > i; i++) 
                    { 
                        Console.WriteLine(d3[a16[i]] + "                    " + a9[i] + "                          " + 
d4[a16[i]]); 
                    } 
                    goto P; 
                } 
                if(a12==2) 
                { 
                    string name, email, str, lan, ci, st, cu, us, p, mob, u1, p1; 
                    int pin; 
                    Console.WriteLine(); 
                    Console.ForegroundColor = ConsoleColor.DarkGreen; 
                    Console.Write("Name      :"); 
                    Console.WriteLine(); 
                    name = Console.ReadLine(); 
(20) 
                V: Console.Write("Contact no :"); 
                    Console.WriteLine(); 
                    mob = Console.ReadLine(); 
                    Regex x = new Regex(pattern); 
                    Console.ForegroundColor = ConsoleColor.Red; 
                    if (x.IsMatch(mob.ToString())) 
                    { 
                        Console.WriteLine("String matched"); 
                    } 
                    else 
                    { 
                        Console.WriteLine("String not matched"); 
                        goto V; 
 
                    } 
                    Console.ForegroundColor = ConsoleColor.DarkGreen; 
                    Console.WriteLine(); 
                N1: Console.Write("Mail Id   : "); 
 
                    email = Console.ReadLine(); 
                    Regex x1 = new Regex(pattern1); 
                    Console.ForegroundColor = ConsoleColor.Red; 
                    if (x1.IsMatch(email)) 
                    { 
                        Console.WriteLine(); 
                        Console.WriteLine("Entered email is in correct format"); 
                    } 
                    else 
                    { 
                        Console.WriteLine("Entered Email is not in Correct format!Please try again"); 
                        goto N1; 
                    } 
                    Console.ForegroundColor = ConsoleColor.DarkGreen; 
                    Console.WriteLine(); 
                    Console.WriteLine("Address:"); 
                    Console.WriteLine(); 
                    Console.Write("Street name :"); 
                    str = Console.ReadLine(); 
                    Console.WriteLine(); 
                    Console.Write("Land mark :"); 
                    lan = Console.ReadLine(); 
                    Console.WriteLine(); 
                    Console.Write("City      :"); 
                    ci = Console.ReadLine(); 
                    Console.WriteLine(); 
                N4: Console.Write("Pincode   :"); 
                    pin = Convert.ToInt32(Console.ReadLine()); 
                    Console.WriteLine(); 
                    Console.ForegroundColor = ConsoleColor.Red; 
                    if (pin.ToString().Length > 7) 
(21) 
                    { 
                        Console.WriteLine("Enter the pin code correctly..."); 
                        goto N4; 
                    } 
                    Console.ForegroundColor = ConsoleColor.DarkGreen; 
 
                    Console.Write("State    :"); 
                    st = Console.ReadLine(); 
                    Console.Write("Country  : "); 
                    cu = Console.ReadLine(); 
                N2: Console.Write("User Id  :"); 
                    us = Console.ReadLine(); 
                    Console.ForegroundColor = ConsoleColor.Red; 
                    if (us.Length > 9) 
                    { 
                        Console.WriteLine("Please Specify Only 8 characters"); 
                        goto N2; 
 
                    } 
                    Console.ForegroundColor = ConsoleColor.DarkGreen; 
                N3: Console.Write("User Password :"); 
                    p = Console.ReadLine(); 
                    Console.ForegroundColor = ConsoleColor.Red; 
                    if (p.Length > 8) 
                    { 
                        Console.WriteLine("Enter password in specified format"); 
                        goto N3; 
                    } 
 
 
                    Console.Clear(); 
                    Console.ForegroundColor = ConsoleColor.Magenta; 
                    Console.WriteLine("WELCOME TO USER LOGIN FORM"); 
                    Console.Write("USER ID         : "); 
                    u1 = Console.ReadLine(); 
                    Console.WriteLine("PASSWORD    :"); 
                    p1 = Console.ReadLine(); 
                    Console.ForegroundColor = ConsoleColor.Green; 
                    if (u1 == us && p1 == p) 
                    { 
                        Console.WriteLine("Logged in Successfully"); 
                        Console.ForegroundColor = ConsoleColor.Magenta; 
                        Console.WriteLine("Name of the item" + "                  " + "Units " + "                           
" + "Cost of the item"); 
                        double total = 0; 
                        Console.ForegroundColor = ConsoleColor.DarkCyan; 
                        for (int i = 0; a16.Length > i; i++) 
                        { 
                            int m, o; 
                            string n; 
(22) 
                            m = d4[a16[i]]; 
                            n = d3[a16[i]]; 
                            o = a9[i]; 
                            total = total + (m * o); 
 
                            Console.WriteLine(n + "                                 " + o + "                               " 
+ m); 
                        } 
 
 
                        double gsta, gst; 
                        gsta = (total * 18) / 100; 
                        gst = total + gsta + gst1; 
                        
Console.WriteLine("===================================================
 ==================================================================
 ==========="); 
                        Console.WriteLine(); 
                        Console.ForegroundColor = ConsoleColor.Yellow; 
                        Console.WriteLine("_ BILLING_"); 
                        Console.WriteLine("Name : " + name); 
                        Console.WriteLine("Contact number" + mob); 
                        Console.WriteLine("NAME OF THE ITEM" + "             " + "UNITS" + "                 
" + "COST OF THE ITEM"); 
                        for (int i = 0; a16.Length > i; i++) 
                        { 
                            int m, o; 
                            string n; 
                            m = d4[a16[i]]; 
                            n = d3[a16[i]]; 
                            o = a9[i]; 
 
 
                            Console.WriteLine(n + "                                   " + o + "                               " 
+ m); 
                        } 
                        Console.WriteLine("-------------------------------------------------------------------------------------------------------------"); 
                        Console.WriteLine("Total:" + "                               " + total); 
                        Console.WriteLine("--------------------------------------------------------------------------------------------------------------"); 
                        Console.WriteLine("GST: 18%"); 
                        Console.WriteLine("---------------------------------------------------------------------------------------------------------------"); 
                        Console.WriteLine("Total Bill:" + "                            " + gst); 
 
                    } 
 
 
                } 
(23) 
            } 
        } 
    }
