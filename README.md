using System;
using System.Collections.Generic;
using System.IO;

class Program
{
    static void Main()
    {
        string ciel1 = "";
        string ciel2 = "";
        string ciel3 = "";

        Random random = new Random();
        int náhoda = random.Next(0, 3);
        string[,] pole = new string[25, 39];
        if (náhoda == 0)
        {
            ciel1 = "C";
            ciel2 = "x";
            ciel3 = "x";
        }
        else if (náhoda == 1)
        {
            ciel1 = "x";
            ciel2 = "C";
            ciel3 = "x";
        }
        else
        {
            ciel1 = "x";
            ciel2 = "x";
            ciel3 = "C";
        }
        int i = 0;
        int y = 9;
        
        while (true)
        {

            Console.WriteLine("Zaciatok" + i);











            // Manuálne naplnenie poľa
            pole[0, 0] = "x";
            pole[0, 1] = "x";
            pole[0, 2] = "x";
            pole[0, 3] = "x";
            pole[0, 4] = "x";
            pole[0, 5] = "x";
            pole[0, 6] = "x";
            pole[0, 7] = "x";
            pole[0, 8] = "x";
            pole[0, 9] = "x";
            pole[0, 10] = ciel1;
            pole[0, 11] = "x";
            pole[0, 12] = "x";
            pole[0, 13] = "x";
            pole[0, 14] = "x";
            pole[0, 15] = "x";
            pole[0, 16] = "x";
            pole[0, 17] = "x";
            pole[0, 18] = "x";
            pole[0, 19] = "x";


            pole[1, 0] = "x";
            pole[1, 1] = " ";
            pole[1, 2] = " ";
            pole[1, 3] = " ";
            pole[1, 4] = " ";
            pole[1, 5] = " ";
            pole[1, 6] = " ";
            pole[1, 7] = " ";
            pole[1, 8] = " ";
            pole[1, 9] = "x";
            pole[1, 10] = " ";
            pole[1, 11] = "x";
            pole[1, 12] = " ";
            pole[1, 13] = " ";
            pole[1, 14] = " ";
            pole[1, 15] = " ";
            pole[1, 16] = " ";
            pole[1, 17] = "x";
            pole[1, 18] = " ";
            pole[1, 19] = "x";

            pole[2, 0] = "x";
            pole[2, 1] = " ";
            pole[2, 2] = "x";
            pole[2, 3] = " ";
            pole[2, 4] = "x";
            pole[2, 5] = "x";
            pole[2, 6] = "x";
            pole[2, 7] = "x";
            pole[2, 8] = " ";
            pole[2, 9] = "x";
            pole[2, 10] = " ";
            pole[2, 11] = "x";
            pole[2, 12] = " ";
            pole[2, 13] = "x";
            pole[2, 14] = " ";
            pole[2, 15] = " ";
            pole[2, 16] = " ";
            pole[2, 17] = "x";
            pole[2, 18] = " ";
            pole[2, 19] = "x";


            pole[3, 0] = "x";
            pole[3, 1] = " ";
            pole[3, 2] = "x";
            pole[3, 3] = " ";
            pole[3, 4] = "x";
            pole[3, 5] = " ";
            pole[3, 6] = " ";
            pole[3, 7] = " ";
            pole[3, 8] = " ";
            pole[3, 9] = "x";
            pole[3, 10] = " ";
            pole[3, 11] = " ";
            pole[3, 12] = " ";
            pole[3, 13] = "x";
            pole[3, 14] = " ";
            pole[3, 15] = " ";
            pole[3, 16] = " ";
            pole[3, 17] = " ";
            pole[3, 18] = " ";
            pole[3, 19] = "x";

            pole[4, 0] = "x";
            pole[4, 1] = "x";
            pole[4, 2] = "x";
            pole[4, 3] = " ";
            pole[4, 4] = "x";
            pole[4, 5] = "x";
            pole[4, 6] = " ";
            pole[4, 7] = "x";
            pole[4, 8] = "x";
            pole[4, 9] = "x";
            pole[4, 10] = " ";
            pole[4, 11] = "x";
            pole[4, 12] = "x";
            pole[4, 13] = "x";
            pole[4, 14] = " ";
            pole[4, 15] = "x";
            pole[4, 16] = "x";
            pole[4, 17] = "x";
            pole[4, 18] = " ";
            pole[4, 19] = "x";


            pole[5, 0] = "x";
            pole[5, 1] = " ";
            pole[5, 2] = " ";
            pole[5, 3] = " ";
            pole[5, 4] = " ";
            pole[5, 5] = "x";
            pole[5, 6] = " ";
            pole[5, 7] = " ";
            pole[5, 8] = " ";
            pole[5, 9] = " ";
            pole[5, 10] = " ";
            pole[5, 11] = "x";
            pole[5, 12] = " ";
            pole[5, 13] = "x";
            pole[5, 14] = " ";
            pole[5, 15] = " ";
            pole[5, 16] = " ";
            pole[5, 17] = " ";
            pole[5, 18] = " ";
            pole[5, 19] = "x";


            pole[6, 0] = "x";
            pole[6, 1] = "x";
            pole[6, 2] = "x";
            pole[6, 3] = "x";
            pole[6, 4] = " ";
            pole[6, 5] = "x";
            pole[6, 6] = "x";
            pole[6, 7] = "x";
            pole[6, 8] = "x";
            pole[6, 9] = "x";
            pole[6, 10] = " ";
            pole[6, 11] = "x";
            pole[6, 12] = " ";
            pole[6, 13] = "x";
            pole[6, 14] = "x";
            pole[6, 15] = "x";
            pole[6, 16] = " ";
            pole[6, 17] = "x";
            pole[6, 18] = "x";
            pole[6, 19] = "x";

            pole[7, 0] = "x";
            pole[7, 1] = "x";
            pole[7, 2] = " ";
            pole[7, 3] = " ";
            pole[7, 4] = " ";
            pole[7, 5] = " ";
            pole[7, 6] = "x";
            pole[7, 7] = " ";
            pole[7, 8] = " ";
            pole[7, 9] = " ";
            pole[7, 10] = " ";
            pole[7, 11] = " ";
            pole[7, 12] = " ";
            pole[7, 13] = "x";
            pole[7, 14] = " ";
            pole[7, 15] = "x";
            pole[7, 16] = " ";
            pole[7, 17] = "x";
            pole[7, 18] = " ";
            pole[7, 19] = "x";


            pole[y-1, 0] = "x";
            pole[y-1, 1] = "x";
            pole[y - 1, 2] = " ";
            pole[y - 1, 3] = "x";
            pole[y - 1, 4] = "x";
            pole[y - 1, 5] = " ";
            pole[y - 1, 6] = "x";
            pole[y - 1, 7] = " ";
            pole[y - 1, 8] = "x";
            pole[y - 1, 9] = "x";
            pole[y - 1, 10] = "x";
            pole[y - 1, 11] = "x";
            pole[y -1, 12] = " ";
            pole[y - 1, 13] = " ";
            pole[y - 1, 14] = " ";
            pole[y -1, 15] = "x";
            pole[y -1, 16] = " ";
            pole[y -1, 17] = "x";
            pole[y -1, 18] = " ";
            pole[y -1, 19] = "x";


            pole[y+0, i] = "H";
            pole[y+0, i+1] = " ";
            pole[y + 0, i+2] = " ";
            pole[y + 0, i+3] = " ";
            pole[y + 0, i+4] = " ";
            pole[y + 0, i+5] = " ";
            pole[y + 0, 6] = "x";
            pole[y + 0, i+7] = " ";
            pole[y + 0, 8] = "x";
            pole[y + 0, i+9] = " ";
            pole[y + 0, i+10] = " ";
            pole[y + 0, 11] = "x";
            pole[y + 0, 12] = "x";
            pole[y + 0, 13] = "x";
            pole[y + 0, i+14] = "O";
            pole[y + 0, 15] = "x";
            pole[y + 0, i+16] = " ";
            pole[y + 0, i+17] = " ";
            pole[y + 0, i+18] = " ";
            pole[9, 19] = ciel2;


            pole[10, 0] = "x";
            pole[10, 1] = "x";
            pole[10, 2] = "x";
            pole[10, 3] = "x";
            pole[10, 4] = "x";
            pole[10, 5] = " ";
            pole[10, 6] = "x";
            pole[10, 7] = " ";
            pole[10, 8] = "x";
            pole[10, 9] = "x";
            pole[10, 10] = "x";
            pole[10, 11] = " ";
            pole[10, 12] = " ";
            pole[10, 13] = "x";
            pole[10, 14] = " ";
            pole[10, 15] = " ";
            pole[10, 16] = " ";
            pole[10, 17] = "x";
            pole[10, 18] = "x";
            pole[10, 19] = "x";


            pole[11, 0] = "x";
            pole[11, 1] = " ";
            pole[11, 2] = " ";
            pole[11, 3] = " ";
            pole[11, 4] = " ";
            pole[11, 5] = " ";
            pole[11, 6] = "x";
            pole[11, 7] = " ";
            pole[11, 8] = " ";
            pole[11, 9] = " ";
            pole[11, 10] = " ";
            pole[11, 11] = " ";
            pole[11, 12] = "x";
            pole[11, 13] = "x";
            pole[11, 14] = "x";
            pole[11, 15] = "x";
            pole[11, 16] = " ";
            pole[11, 17] = "x";
            pole[11, 18] = " ";
            pole[11, 19] = "x";


            pole[12, 0] = "x";
            pole[12, 1] = " ";
            pole[12, 2] = "x";
            pole[12, 3] = "x";
            pole[12, 4] = "x";
            pole[12, 5] = " ";
            pole[12, 6] = "x";
            pole[12, 7] = " ";
            pole[12, 8] = "x";
            pole[12, 9] = "x";
            pole[12, 10] = "x";
            pole[12, 11] = "x";
            pole[12, 12] = "x";
            pole[12, 13] = "x";
            pole[12, 14] = " ";
            pole[12, 15] = " ";
            pole[12, 16] = " ";
            pole[12, 17] = " ";
            pole[12, 18] = " ";
            pole[12, 19] = "x";


            pole[13, 0] = "x";
            pole[13, 1] = " ";
            pole[13, 2] = "x";
            pole[13, 3] = " ";
            pole[13, 4] = "x";
            pole[13, 5] = " ";
            pole[13, 6] = " ";
            pole[13, 7] = " ";
            pole[13, 8] = "x";
            pole[13, 9] = " ";
            pole[13, 10] = " ";
            pole[13, 11] = " ";
            pole[13, 12] = " ";
            pole[13, 13] = " ";
            pole[13, 14] = " ";
            pole[13, 15] = "x";
            pole[13, 16] = " ";
            pole[13, 17] = "x";
            pole[13, 18] = " ";
            pole[13, 19] = "x";


            pole[14, 0] = "x";
            pole[14, 1] = " ";
            pole[14, 2] = " ";
            pole[14, 3] = " ";
            pole[14, 4] = "x";
            pole[14, 5] = "x";
            pole[14, 6] = "x";
            pole[14, 7] = "x";
            pole[14, 8] = "x";
            pole[14, 9] = " ";
            pole[14, 10] = "x";
            pole[14, 11] = " ";
            pole[14, 12] = "x";
            pole[14, 13] = "x";
            pole[14, 14] = " ";
            pole[14, 15] = "x";
            pole[14, 16] = "x";
            pole[14, 17] = "x";
            pole[14, 18] = "x";
            pole[14, 19] = "x";

            pole[15, 0] = "x";
            pole[15, 1] = "x";
            pole[15, 2] = "x";
            pole[15, 3] = " ";
            pole[15, 4] = " ";
            pole[15, 5] = " ";
            pole[15, 6] = " ";
            pole[15, 7] = " ";
            pole[15, 8] = " ";
            pole[15, 9] = " ";
            pole[15, 10] = "x";
            pole[15, 11] = " ";
            pole[15, 12] = " ";
            pole[15, 13] = " ";
            pole[15, 14] = " ";
            pole[15, 15] = " ";
            pole[15, 16] = " ";
            pole[15, 17] = " ";
            pole[15, 18] = " ";
            pole[15, 19] = "x";


            pole[16, 0] = "x";
            pole[16, 1] = " ";
            pole[16, 2] = "x";
            pole[16, 3] = "x";
            pole[16, 4] = "x";
            pole[16, 5] = " ";
            pole[16, 6] = "x";
            pole[16, 7] = "x";
            pole[16, 8] = "x";
            pole[16, 9] = "x";
            pole[16, 10] = "x";
            pole[16, 11] = "x";
            pole[16, 12] = "x";
            pole[16, 13] = "x";
            pole[16, 14] = " ";
            pole[16, 15] = "x";
            pole[16, 16] = " ";
            pole[16, 17] = "x";
            pole[16, 18] = " ";
            pole[16, 19] = "x";


            pole[17, 0] = "x";
            pole[17, 1] = " ";
            pole[17, 2] = "x";
            pole[17, 3] = " ";
            pole[17, 4] = "x";
            pole[17, 5] = " ";
            pole[17, 6] = "x";
            pole[17, 7] = " ";
            pole[17, 8] = " ";
            pole[17, 9] = " ";
            pole[17, 10] = " ";
            pole[17, 11] = " ";
            pole[17, 12] = " ";
            pole[17, 13] = "x";
            pole[17, 14] = "x";
            pole[17, 15] = "x";
            pole[17, 16] = " ";
            pole[17, 17] = "x";
            pole[17, 18] = " ";
            pole[17, 19] = "x";


            pole[18, 0] = "x";
            pole[18, 1] = " ";
            pole[18, 2] = " ";
            pole[18, 3] = " ";
            pole[18, 4] = " ";
            pole[18, 5] = " ";
            pole[18, 6] = "x";
            pole[18, 7] = " ";
            pole[18, 8] = "x";
            pole[18, 9] = "x";
            pole[18, 10] = " ";
            pole[18, 11] = "x";
            pole[18, 12] = " ";
            pole[18, 13] = " ";
            pole[18, 14] = " ";
            pole[18, 15] = " ";
            pole[18, 16] = " ";
            pole[18, 17] = "x";
            pole[18, 18] = " ";
            pole[18, 19] = "x";


            pole[19, 0] = "x";
            pole[19, 1] = "x";
            pole[19, 2] = "x";
            pole[19, 3] = "x";
            pole[19, 4] = "x";
            pole[19, 5] = "x";
            pole[19, 6] = "x";
            pole[19, 7] = "x";
            pole[19, 8] = "x";
            pole[19, 9] = "x";
            pole[19, 10] = ciel3;
            pole[19, 11] = "x";
            pole[19, 12] = "x";
            pole[19, 13] = "x";
            pole[19, 14] = "x";
            pole[19, 15] = "x";
            pole[19, 16] = "x";
            pole[19, 17] = "x";
            pole[19, 18] = "x";
            pole[19, 19] = "x";

            for (int riadok = 0; riadok < pole.GetLength(0); riadok++)
            {
                for (int stlpec = 0; stlpec < pole.GetLength(1); stlpec++)
                {
                    Console.Write(pole[riadok, stlpec] + "    ");
                }
                Console.WriteLine();


            }

            string pohyb = Console.ReadLine();
            if (pohyb == "d")
            {
                pole[9, i] = " ";
                i++;
                
                pole[9, i] = "H";

            }


            if (pohyb == "a")
            {
                pole[9, i] = " ";
                i--;

                pole[9, i] = "H";
            }


            if (pohyb == "w")
            {
                pole[9, y] = " ";
                y++;

                pole[9, y] = "H";
            }


            if (pohyb == "s")
            {
                pole[9, y] = " ";
                y--;

                pole[9, y] = "H";
            }
            Console.WriteLine("Koniec y " + y);
            Console.WriteLine("Koniec i " + i);
        }




    }
}
