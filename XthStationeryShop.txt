import java.io.*;
public class Empl
{
  public static void main(String args[]) throws IOException
  {   
    int finalamt=0,purchaseyn,bluebrand,blackbrand,redbrand,othcolmarksketchbrand,bbrand,orderabrand,prinkerabrand,notsinhafbrand,notsinfulbrand,notdobbrand;
    int b3brand,hbrand,h2brand,h3brand,hbbrand,cmbbrand,nottribrand,notsqrbrand,notdraa3brand,notdraa4brand,geoboxbrand,geospcombrand,geospdivbrand;
    int geosprulbbrand,geosprulsbrand,b2brand;
    String chink;
    
    InputStreamReader read=new InputStreamReader(System.in);
    BufferedReader in=new BufferedReader(read);
    System.out.println( "                                             W                     W  EEEE  L       CCCC  OOOO  MM        M M  EEEE  ");
    System.out.println( "                                               W        W       W   E       L       C          O      O  M M      M M  E     ");
    System.out.println( "                                                 W    W W   W    EEE   L       C         O       O  M   M  M   EEE   ");
    System.out.println( "                                                   W W   W W     E       L        C         O      O  M       M           E     ");
    System.out.println( "                                                      W       W       EEEE  LLLL  CCCC  OOOO  M               M  EEEE  ");
    System.out.println();
    System.out.println( "                                                                               TTTTT  OOO");
    System.out.println( "                                                                                   T       O  O");
    System.out.println( "                                                                                 T    OOO");
    System.out.println();
    System.out.println( "                                                         RRRR  U   U  L     W                 W  III  NN    N");
    System.out.println( "                                                         R     R  U   U  L      W               W    I   N N   N");
    System.out.println( "                                                         RRRR  U    U  L       W     W    W     I   N  N  N");
    System.out.println( "                                                         R  R    U      U  L        W W W W     I   N   N N");
    System.out.println( "                                                         R    R  UUUU  LLLL      W     W       III  N    NN");
    System.out.println( );
    System.out.println( "                                                          RULE THE ARC.           GET THE MARK   ");
    System.out.println();
    System.out.println();
    System.out.println(" Enter your name " );
    String customername=in.readLine();
    do{
        System.out.println("Please choose your category --" );
        System.out.println("1. Pens" );
        System.out.println("2. Pencils" );
        System.out.println("3. Erasers" );
        System.out.println("4. Notebooks" );
        System.out.println("5. Geometry kits and tools" );
        System.out.println("6. Other than these" );
        String choice=in.readLine();
        if(choice.equalsIgnoreCase("pens") || choice.equals("1") || choice.equalsIgnoreCase("pen"))
        {
          System.out.println("please select the ink color needed" );
          System.out.println("1.blue");
          System.out.println("2.black");
          System.out.println("3.red");
          System.out.println("4.other colour/markers/sketch pens");
          chink=in.readLine();
          if(chink.equalsIgnoreCase("blue")||choice.equals("1"))
          {
           String blue[]={"Linc","ADD","cello","Flair","Parker","Reynolds"};
           int bluecost[]={5,25,10,15,40,15};
           do{
              System.out.println("Please choose brand number");
              for(int i=0;i<6;i++)
              {
               System.out.println( (i+1)+ "." +blue[i]); 
              }
              bluebrand=Integer.parseInt(in.readLine());
            }while(bluebrand>=6);
           System.out.println("Please enter number of pens");
           int blueno=Integer.parseInt(in.readLine());
           finalamt = finalamt + (blueno * bluecost[bluebrand-1]);
           }
           else if(chink.equalsIgnoreCase("black")||choice.equals("2"))
           {
            String black[]= {"Linc","ADD","cello","Flair","Parker","Reynolds"};
            int blackcost[]={5,25,10,15,40,15};
           do{
            System.out.println("Please choose brand number");
            for(int i=0;i<6;i++)
            {
              System.out.println( (i+1)+ "." +black[i]); 
             }
            blackbrand=Integer.parseInt(in.readLine());
             }while(blackbrand>=6);
           System.out.println("Please enter number of pens");
           int blackno=Integer.parseInt(in.readLine());
           finalamt=finalamt+(blackno * blackcost[blackbrand-1]); 
           }   
          else if(chink.equalsIgnoreCase("red")||choice.equals("3"))
          {
            String red[]= {"Linc","ADD","cello","Flair","Parker","Reynolds"};
            int redcost[]={5,25,10,15,40,15};
            do{
               System.out.println("Please choose brand number");
              for(int i=0;i<6;i++)
              {
                System.out.println((i+1)+"."+red[i]); 
               }
              redbrand=Integer.parseInt(in.readLine());
              }while(redbrand>=6);
            System.out.println("Please enter number of pens");
            int redno=Integer.parseInt(in.readLine());
            finalamt = finalamt + (redno * redcost[redbrand-1]);
             }
          else if(chink.equalsIgnoreCase("other colour")||choice.equals("4")||chink.equalsIgnoreCase("markers")||chink.equalsIgnoreCase("sketch pens"))
          {
            String othcolmarksketch[]={"green pen","camlin sketch pen set(10 pc)","Nataraj sketch pen set(15 pc)" };
            int othcolmarksketchcost[]={15,50,75,};
           do{
              System.out.println("Please choose brand number");
             for(int i=0;i<3;i++)
             {
              System.out.println((i+1)+"."+othcolmarksketch[i]); 
              }
             othcolmarksketchbrand=Integer.parseInt(in.readLine());
             }while(othcolmarksketchbrand>=3);
           System.out.println("Please enter number of pens");
           int othcolmarksketchno=Integer.parseInt(in.readLine());
           finalamt = finalamt + (othcolmarksketchno * othcolmarksketchcost[othcolmarksketchbrand-1]);
             }   
            else
            {
                System.out.println("Incorrect item selected.please log-in again");
         }
           
        }
        else if(choice.equalsIgnoreCase("pencils") || choice.equals("2") || choice.equalsIgnoreCase("pencil"))
          {
          System.out.println("Please select pencil quality");//h,2h,3h,b,2b,3b,hb,fullpack
          System.out.println("1.Bold            (B)");
          System.out.println("2.Double Bold    (2B)");
          System.out.println("3.Triple Bold    (3B)");
          System.out.println("4.Hard            (H)");
          System.out.println("5.Double Hard    (2H)");
          System.out.println("6.Triple Hard    (3H)");
          System.out.println("7.Hard and Bold  (HB)");
          System.out.println("8.Combo Packs(contains 1 pc. of all of the above)");
          String chleadqua=in.readLine();
          if(chleadqua.equals("1")||chleadqua.equalsIgnoreCase("bold")||chleadqua.equalsIgnoreCase("b"))
         {
           String b[]= {"Nataraj","Camlin","Apsara","Flora"};
           int bcost[]={2,5,5,7};
           do{
             System.out.println("Please choose brand number");
             for(int i=0;i<4;i++)
             {
               System.out.println((i+1)+"."+b[i]); 
              }
             bbrand=Integer.parseInt(in.readLine());
              }while(bbrand>=4);
                System.out.println("Please enter number of pencils");
                int bno=Integer.parseInt(in.readLine());
                finalamt = finalamt + (bno * bcost[bbrand-1]);
                }
          else if(chleadqua.equals("2")||chleadqua.equalsIgnoreCase("double bold")||chleadqua.equalsIgnoreCase("2b"))
              {
                 String b2[]= {"Nataraj","Camlin","Apsara","Flora"};
               int b2cost[]={4,7,8,9};
               do{
                System.out.println("Please choose brand number");
                for(int i=0;i<4;i++)
                {
                  System.out.println((i+1)+"."+b2[i]); 
                }
                b2brand=Integer.parseInt(in.readLine());
               }while(b2brand>=4);
               System.out.println("Please enter number of pencils");
               int b2no=Integer.parseInt(in.readLine());
               finalamt = finalamt + (b2no * b2cost[b2brand-1]);
                }
              else if(chleadqua.equals("3")||chleadqua.equalsIgnoreCase("triple bold")||chleadqua.equalsIgnoreCase("3b"))
              {
                 String b3[]= {"Nataraj","Camlin","Apsara","Flora"};
               int b3cost[]={6,14,12,10};
               do{
                System.out.println("Please choose brand number");
                for(int i=0;i<4;i++)
                {
                 System.out.println((i+1)+"."+b3[i]); 
                }
                b3brand=Integer.parseInt(in.readLine());
                }while(b3brand>=4);
                System.out.println("Please enter number of pencils");
               int b3no=Integer.parseInt(in.readLine());
               finalamt = finalamt + (b3no * b3cost[b3brand-1]);
                }
              else if(chleadqua.equals("4")||chleadqua.equalsIgnoreCase("hard")||chleadqua.equalsIgnoreCase("h"))
              {
                 String h[]= {"Nataraj","Camlin","Apsara","Flora"};
               int hcost[]={3,4,5,4};
                do{
                 System.out.println("Please choose brand number");
                 for(int i=0;i<4;i++)
                 {
                 System.out.println((i+1)+"."+h[i]); 
                 }
                 hbrand=Integer.parseInt(in.readLine());
                }while(hbrand>=4);
                System.out.println("Please enter number of pencils");
               int hno=Integer.parseInt(in.readLine());
               finalamt = finalamt + (hno * hcost[hbrand-1]);
                }
              else if(chleadqua.equals("5")||chleadqua.equalsIgnoreCase("double hard")||chleadqua.equalsIgnoreCase("2h"))
              {
                String h2[]= {"Nataraj","Camlin","Apsara","Flora"};
               int h2cost[]={6,7,9,8};
                do{
                 System.out.println("Please choose brand number");
                 for(int i=0;i<4;i++)
                 {
                 System.out.println((i+1)+"."+h2[i]); 
                 }
                 h2brand=Integer.parseInt(in.readLine());
               }while(h2brand>=4);
                 System.out.println("Please enter number of pencils");
               int h2no=Integer.parseInt(in.readLine());
               finalamt = finalamt + (h2no * h2cost[h2brand-1]);
                }
              else if(chleadqua.equals("6")||chleadqua.equalsIgnoreCase("triple hard")||chleadqua.equalsIgnoreCase("3h"))
              {
                String h3[]= {"Nataraj","Camlin","Apsara","Flora"};
               int h3cost[]={9,12,15,10};
                do{
                 System.out.println("Please choose brand number");
                 for(int i=0;i<4;i++)
                 {
                  System.out.println((i+1)+"."+h3[i]); 
                 }
                 h3brand=Integer.parseInt(in.readLine());
               }while(h3brand>=4);
                 System.out.println("Please enter number of pencils");
               int h3no=Integer.parseInt(in.readLine());
               finalamt = finalamt + (h3no * h3cost[h3brand-1]);
                }
              else if(chleadqua.equals("7")||chleadqua.equalsIgnoreCase("hard and bold")||chleadqua.equalsIgnoreCase("hb"))
              {
                String hb[]= {"Nataraj","Camlin","Apsara","Flora"};
               int hbcost[]={5,8,7,6};
                do{
                System.out.println("Please choose brand number");
                for(int i=0;i<4;i++)
                {
                 System.out.println((i+1)+"."+hb[i]); 
                }
                hbbrand=Integer.parseInt(in.readLine());
               }while(hbbrand>=4);
                System.out.println("Please enter number of pencils");
               int hbno=Integer.parseInt(in.readLine());
               finalamt = finalamt + (hbno * hbcost[hbbrand-1]);
                }
              else if(chleadqua.equals("8")||chleadqua.equalsIgnoreCase("combo pack"))
              {
                String cmb[]= {"Nataraj","Camlin","Apsara","Flora"};
               int cmbcost[]={49,40,45,39};
                do{
                 System.out.println("Please choose brand number");
                 for(int i=0;i<4;i++)
                 {
                  System.out.println((i+1)+"."+cmb[i]); 
                 }
                 cmbbrand=Integer.parseInt(in.readLine());
                }while(cmbbrand>=4);
                System.out.println("Please enter number of pencils");
               int cmbno=Integer.parseInt(in.readLine());
               finalamt = finalamt + (cmbno * cmbcost[cmbbrand-1]);
                }
              else
         {
          System.out.println("incorrect item selected.please log in again");
         }
         }
        else if(choice.equalsIgnoreCase("erasers") || choice.equals("3") || choice.equalsIgnoreCase("eraser"))    
        {
         System.out.println("Please select eraser quality");
         System.out.println("1.Ordinary Erasers");
         System.out.println("2.Ink/Print Erasers");
         String chquaeras=in.readLine();
         if(chquaeras.equalsIgnoreCase("ordinary") || chquaeras.equals("1") || chquaeras.equalsIgnoreCase("ordinary erasers"))
         {
            String ordera[]= {"Nataraj","Camlin","Apsara","Kiddo"};
            int orderacost[]={2,4,5,2};
            do{
             System.out.println("Please choose brand number");
             for(int i=0;i<4;i++)
             {
               System.out.println((i+1)+"."+ordera[i]); 
              }
             orderabrand=Integer.parseInt(in.readLine());
              }while(orderabrand>4);
            System.out.println("Please enter number of erasers");
            int orderano=Integer.parseInt(in.readLine());
            finalamt = finalamt + (orderano * orderacost[orderabrand-1]);
          }
         else if(chquaeras.equalsIgnoreCase("ink")||chquaeras.equals("2")||chquaeras.equalsIgnoreCase("ink eraser")||chquaeras.equalsIgnoreCase("print")||chquaeras.equalsIgnoreCase("print eraser"))
         {
             String prinkera[]= {"Nataraj","Camlin","Apsara","Stedlear"};
            int prinkeracost[]={10,14,12,15};
            do{
             System.out.println("Please choose brand number");
             for(int i=0;i<4;i++)
             {
               System.out.println((i+1)+"."+prinkera[i]); 
              }
             prinkerabrand=Integer.parseInt(in.readLine());
              }while(prinkerabrand>4);
            System.out.println("Please enter number of erasers");
            int prinkerano=Integer.parseInt(in.readLine());
            finalamt = finalamt + (prinkerano * prinkeracost[prinkerabrand-1]);
          }
         else
         {
           System.out.println("incorrect item selected.please log in again");
          } 
         }
        else if(choice.equalsIgnoreCase("notebooks") || choice.equals("4") || choice.equalsIgnoreCase("notebook"))
        {
          System.out.println("Please select the type of notebooks");
          System.out.println("1.Single lined");
          System.out.println("2.Double lined");
          System.out.println("3.Triple lined(red and blue lined)");
          System.out.println("4.Square lined"); 
          System.out.println("5.Drawing book");//and graph books
          System.out.println("6.Sketch book(blank and ruled pages)");
          System.out.println("7.Graph book");
          String chnotetyp=in.readLine();
          if(chnotetyp.equalsIgnoreCase("Single") || chnotetyp.equals("1") || choice.equalsIgnoreCase("single lined"))
          {
            System.out.println("Please select the size of notebooks");
            System.out.println("1.Half scape");
            System.out.println("2.Full scape");
            String chnotsinsiz=in.readLine();
            if(chnotsinsiz.equalsIgnoreCase("half") || chnotsinsiz.equals("1") || chnotsinsiz.equalsIgnoreCase("half scape"))
           {
            String notsinhaf[]= {"Sundaram","Classmate","Navneet","Mr.Big","Runner","Crazy World"};
            int notsinhafcost[]={18,19,18,20,18,16};
            do{
             System.out.println("Please choose brand number");
             for(int i=0;i<6;i++)
             {
               System.out.println((i+1)+"."+notsinhaf[i]); 
              }
             notsinhafbrand=Integer.parseInt(in.readLine());
              }while(notsinhafbrand>6);
            System.out.println("Please enter number of notebooks");
            int notsinhafno=Integer.parseInt(in.readLine());
            finalamt = finalamt + (notsinhafno * notsinhafcost[notsinhafbrand-1]);
           }
           else if(chnotsinsiz.equalsIgnoreCase("full") || chnotsinsiz.equals("2") || chnotsinsiz.equalsIgnoreCase("full scape"))
           {
            String notsinful[]= {"Sundaram","Classmate","Navneet","Mr.Big","Runner","Crazy World"};
            int notsinfulcost[]={36,37,35,40,36,33};
            do{
             System.out.println("Please choose brand number");
             for(int i=0;i<6;i++)
             {
               System.out.println((i+1)+"."+notsinful[i]); 
              }
             notsinfulbrand=Integer.parseInt(in.readLine());
              }while(notsinfulbrand>6);
            System.out.println("Please enter number of notebooks");
            int notsinfulno=Integer.parseInt(in.readLine());
            finalamt = finalamt + (notsinfulno * notsinfulcost[notsinfulbrand-1]);
           }
            }
          else if(chnotetyp.equalsIgnoreCase("Double") || chnotetyp.equals("2") || choice.equalsIgnoreCase("double lined"))
          {
            String notdob[]= {"Sundaram","Classmate","Navneet","Mr.Big","Runner","Crazy World"};
            int notdobcost[]={18,19,18,20,18,16};
            do{
             System.out.println("Please choose brand number");
             for(int i=0;i<6;i++)
             {
               System.out.println((i+1)+"."+notdob[i]); 
              }
             notdobbrand=Integer.parseInt(in.readLine());
              }while(notdobbrand>6);
            System.out.println("Please enter number of notebooks");
            int notdobno=Integer.parseInt(in.readLine());
            finalamt = finalamt + (notdobno * notdobcost[notdobbrand-1]);
           }
          else if(chnotetyp.startsWith("Triple") || chnotetyp.equals("3") || choice.startsWith("red and blue"))
          {
            String nottri[]= {"Sundaram","Classmate","Navneet","Mr.Big","Runner","Crazy World"};
            int nottricost[]={18,19,18,20,18,16};
            do{
             System.out.println("Please choose brand number");
             for(int i=0;i<6;i++)
             {
               System.out.println((i+1)+"."+nottri[i]); 
              }
             nottribrand=Integer.parseInt(in.readLine());
              }while(nottribrand>6);
            System.out.println("Please enter number of notebooks");
            int nottrino=Integer.parseInt(in.readLine());
            finalamt = finalamt + (nottrino * nottricost[nottribrand-1]);
            }
            else if(chnotetyp.startsWith("square") || chnotetyp.equals("4"))
            {
              String notsqr[]= {"Sundaram","Classmate","Navneet","Mr.Big","Runner","Crazy World"};
               int notsqrcost[]={18,19,18,20,18,16};
            do{
                System.out.println("Please choose brand number");
                for(int i=0;i<6;i++)
                {
                  System.out.println((i+1)+"."+notsqr[i]); 
                 }
              notsqrbrand=Integer.parseInt(in.readLine());
                 }while(notsqrbrand>6);
               System.out.println("Please enter number of notebooks");
               int notsqrno=Integer.parseInt(in.readLine());
               finalamt = finalamt + (notsqrno * notsqrcost[notsqrbrand-1]);
             }
             else if(chnotetyp.startsWith("drawing") || chnotetyp.equals("5"))
             {
              System.out.println("Please select the size of notebooks");
              System.out.println("1.Half scape");
              System.out.println("2.A-3 size");
              System.out.println("2.A-4 size");
              String chnotdrasiz=in.readLine();
              if(chnotdrasiz.startsWith("half")||chnotdrasiz.equals("1"))
              {
                int notdrahafcost=15;
                System.out.println("Please enter number of notebooks");
                 int notdrahafno=Integer.parseInt(in.readLine());
                finalamt = finalamt + (notdrahafno * notdrahafcost);
                }
            else if(chnotdrasiz.startsWith("a-3")||chnotdrasiz.equals("2")||chnotdrasiz.startsWith("A-3"))
              {
              String notdraa3[]= {"Sundaram","Navneet"};
              int notdraa3cost[]={46,49};
              do{
                  System.out.println("Please choose brand number");
                   for(int i=0;i<2;i++)
                   {
                    System.out.println((i+1)+"."+notdraa3[i]); 
                    }
                   notdraa3brand=Integer.parseInt(in.readLine());
                 }while(notdraa3brand>6);
              System.out.println("Please enter number of notebooks");
              int notdraa3no=Integer.parseInt(in.readLine());
              finalamt = finalamt + (notdraa3no * notdraa3cost[notdraa3brand-1]);
                }
            else if(chnotdrasiz.startsWith("a-4")||chnotdrasiz.equals("3")||chnotdrasiz.startsWith("A-4"))
              {
              String notdraa4[]= {"Sundaram","Navneet"};
              int notdraa4cost[]={46,49};
              do{
                  System.out.println("Please choose brand number");
                   for(int i=0;i<2;i++)
                   {
                    System.out.println((i+1)+"."+notdraa4[i]); 
                    }
                   notdraa4brand=Integer.parseInt(in.readLine());
                 }while(notdraa4brand>2);
              System.out.println("Please enter number of notebooks");
              int notdraa4no=Integer.parseInt(in.readLine());
              finalamt = finalamt + (notdraa4no * notdraa4cost[notdraa4brand-1]);
                }    
                }
           else if(chnotetyp.equalsIgnoreCase("sketch") || chnotetyp.equals("6")||chnotetyp.equalsIgnoreCase("sketch book"))
           {
            System.out.println("Please select the type of notebooks");
            System.out.println("1.Notebook type(half scape,soft cover)");
            System.out.println("2.Journal type(full scape,hard cover)");
            String chnotsketyp=in.readLine();
             if(chnotsketyp.startsWith("notebook") || chnotetyp.equals("1")||chnotsketyp.startsWith("half")||chnotsketyp.startsWith("soft"))
             {
               int notskehafcost=20; 
                System.out.println("Please enter number of notebooks");
                 int notskehafno=Integer.parseInt(in.readLine());
                finalamt = finalamt + (notskehafno * notskehafcost);
              }
            else if(chnotsketyp.startsWith("journal") || chnotetyp.equals("2")||chnotsketyp.startsWith("full")||chnotsketyp.startsWith("hard"))
             {
              int notskefulcost=20; 
                System.out.println("Please enter number of notebooks");
                 int notskefulno=Integer.parseInt(in.readLine());
                finalamt = finalamt + (notskefulno * notskefulcost);
              }  
            }
          else if(chnotetyp.startsWith("graph") || chnotetyp.equals("7"))
           { 
             int notgracost=20; 
             System.out.println("Please enter number of notebooks");
             int notgrano=Integer.parseInt(in.readLine());
             finalamt = finalamt + (notgrano * notgracost);
            }  
        }
        else if(choice.startsWith("geometry")||choice.equals("5"))
        {
          System.out.println("Please choose type of purchase ");
          System.out.println("1.Complete geometry box");
          System.out.println("2.Spare geometric tools");
          String chgeopur=in.readLine();
          if(chgeopur.startsWith("complete")||chgeopur.startsWith("1")||chgeopur.startsWith("geometry"))
              {
              String geobox[]= {"Natraj","Camlin","Apsara","Faber-Castle"};
              int geoboxcost[]={40,45,49,45};
              do{
                  System.out.println("Please choose brand number");
                   for(int i=0;i<4;i++)
                   {
                    System.out.println((i+1)+"."+geobox[i]); 
                    }
                   geoboxbrand=Integer.parseInt(in.readLine());
                 }while(geoboxbrand>4);
              System.out.println("Please enter number of notebooks");
              int geoboxno=Integer.parseInt(in.readLine());
              finalamt = finalamt + (geoboxno * geoboxcost[geoboxbrand-1]);
                } 
          else if(chgeopur.startsWith("spare")||chgeopur.startsWith("2")||chgeopur.startsWith("geometric"))
          {
            System.out.println("Please select the item to be purchased-");
            System.out.println("1.Compass");
            System.out.println("2.Divider");
            System.out.println("3.Set squares(30-60-90 & 45-90) and protactor");
            System.out.println("4.Procircle");
            System.out.println("5.French curve");
            System.out.println("6.Ruler");
            System.out.println("7.Stencils");
            String chgeosp=in.readLine();
            if(chgeosp.equalsIgnoreCase("compass")||chgeosp.equals("1"))
            {  
              String geospcom[]= {"Natraj","Camlin","Apsara","Faber-Castle","Maped"};
              int geospcomcost[]={25,30,25,20,45};
              do{
                  System.out.println("Please choose brand number");
                   for(int i=0;i<5;i++)
                   {
                    System.out.println((i+1)+"."+geospcom[i]); 
                    }
                   geospcombrand=Integer.parseInt(in.readLine());
                 }while(geospcombrand>5);
              System.out.println("Please enter number of compasses");
              int geospcomno=Integer.parseInt(in.readLine());
              finalamt = finalamt + (geospcomno * geospcomcost[geospcombrand-1]); 
             }
            else if(chgeosp.equalsIgnoreCase("divider")||chgeosp.equals("2"))
            {  
              String geospdiv[]= {"Natraj","Camlin","Apsara","Faber-Castle","Maped"};
              int geospdivcost[]={25,30,25,20,45};
              do{
                  System.out.println("Please choose brand number");
                   for(int i=0;i<5;i++)
                   {
                    System.out.println((i+1)+"."+geospdiv[i]); 
                    }
                   geospdivbrand=Integer.parseInt(in.readLine());
                 }while(geospdivbrand>5);
              System.out.println("Please enter number of dividers");
              int geospdivno=Integer.parseInt(in.readLine());
              finalamt = finalamt + (geospdivno * geospdivcost[geospdivbrand-1]); 
             }
            else if(chgeosp.startsWith("set")||chgeosp.equals("3")||chgeosp.startsWith("protractor")) 
            {
              int geospsspcost=10;
              System.out.println("Please enter number of kits");
              int geospsspno=Integer.parseInt(in.readLine());
              finalamt = finalamt + (geospsspno * geospsspcost);
             }
            else if(chgeosp.equalsIgnoreCase("procircle")||chgeosp.equals("4")) 
            {
              int geospprccost=12;
              System.out.println("Please enter number of procircles");
              int geospprcno=Integer.parseInt(in.readLine());
              finalamt = finalamt + (geospprcno * geospprccost);
             }
            else if(chgeosp.startsWith("french")||chgeosp.equals("5")) 
            {
              int geospfrccost=12;
              System.out.println("Please enter number of french curves");
              int geospfrcno=Integer.parseInt(in.readLine());
              finalamt = finalamt + (geospfrcno * geospfrccost);
             }
            else if(chgeosp.startsWith("ruler")||chgeosp.equals("6")) 
            {  
              System.out.println("please select length of ruler");
              System.out.println("1.15cm/6inches");
              System.out.println("2.30cm/12inches");
              System.out.println("3.1m");
              String chgeorullen=in.readLine();
              if(chgeorullen.startsWith("15")||chgeorullen.equals("1")||chgeorullen.startsWith("6"))
              {    
                String geospruls[]= {"Natraj","Camlin","Apsara","Faber-Castle","steel type"};
               int geosprulscost[]={4,5,6,3,10};
               do{
                  System.out.println("Please choose brand number");
                   for(int i=0;i<5;i++)
                   {
                    System.out.println((i+1)+"."+geospruls[i]); 
                    }
                   geosprulsbrand=Integer.parseInt(in.readLine());
                 }while(geosprulsbrand>5);
               System.out.println("Please enter number of rulers");
               int geosprulsno=Integer.parseInt(in.readLine());
               finalamt = finalamt + (geosprulsno * geosprulscost[geosprulsbrand-1]);   
                }
              else if(chgeorullen.startsWith("30")||chgeorullen.equals("2")||chgeorullen.startsWith("12"))
              {    
                String geosprulb[]= {"Natraj","Camlin","Apsara","Faber-Castle","steel type"};
               int geosprulbcost[]={8,10,12,9,20};
               do{
                  System.out.println("Please choose brand number");
                   for(int i=0;i<5;i++)
                   {
                    System.out.println((i+1)+"."+geosprulb[i]); 
                    }
                   geosprulbbrand=Integer.parseInt(in.readLine());
                 }while(geosprulbbrand>5);
               System.out.println("Please enter number of rulers");
               int geosprulbno=Integer.parseInt(in.readLine());
               finalamt = finalamt + (geosprulbno * geosprulbcost[geosprulbbrand-1]);   
                }
              else if(chgeorullen.startsWith("1")||chgeorullen.equals("2"))
              {  
                int geosprulmcost=40;
                System.out.println("Please enter number of rulers");
               int geosprulmno=Integer.parseInt(in.readLine());
               finalamt = finalamt + (geosprulmno * geosprulmcost);
                }
             }
            else if(chgeosp.startsWith("stencil")||chgeosp.equals("7"))
            { 
               System.out.println("Please select type of stencil-");
               System.out.println("1.Alphabet stencil");
               System.out.println("2.Shape stencil");
               System.out.println("3.Chemistry-diagram stencil");
               String chgeospstentyp=in.readLine();
               if(chgeospstentyp.startsWith("alphabet")||chgeospstentyp.equals("1"))
               { 
                int geospstenacost=10;
                System.out.println("Please enter number of stencils");
                int geospstenano=Integer.parseInt(in.readLine());
                finalamt = finalamt + (geospstenano * geospstenacost);
                }
               else if(chgeospstentyp.startsWith("shape")||chgeospstentyp.equals("2"))
               { 
                int geospstenscost=20;
                System.out.println("Please enter number of stencils");
                int geospstensno=Integer.parseInt(in.readLine());
                finalamt = finalamt + (geospstensno * geospstenscost);
                }
               else if(chgeospstentyp.startsWith("chemistry")||chgeospstentyp.equals("3"))
               { 
                int geospstenccost=20;
                System.out.println("Please enter number of stencils");
                int geospstencno=Integer.parseInt(in.readLine());
                finalamt = finalamt + (geospstencno * geospstenccost);
                }                
             }
            }    
         }
        else if(choice.startsWith("other")||choice.equals("6"))
        { 
          System.out.println("Please name the desired item:");
          String desireditem=in.readLine();
          System.out.println("Your"+desireditem+"will be available at our shop within 2 weeks from today");  
         }
        System.out.println("would you like to purchase anything else?" ); 
        System.out.println("1.yes" );
        System.out.println("2.no" );
        purchaseyn=Integer.parseInt(in.readLine());
      }while( purchaseyn==1);
      
      System.out.println();    
      System.out.println("Name- "+customername); 
      System.out.println("Price = Rs."+finalamt+"(inclusive of all purchases)");
      System.out.println("                                                      THANK YOU !!!" );
      
    }
}
//end of program