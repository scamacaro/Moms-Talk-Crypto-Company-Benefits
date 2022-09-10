# Moms-Talk-Crypto-Company-Benefits
Assignment: Startup Company Benefits - CSC202
/*
 Sanyerlis Camacaro 09/12/2022 - CSC202 - Startup Company - Moms Talk Crypto Company Benefits - Sancamac@uat.edu
Log: As of September 8,2022 I believe this project will take me to complete in less than 8 hours splitted in 2-3 days.
09/09/2022 Started rewatching the class to follow along with the examples, Starting time was at 10:43am, I've finished following along the class video around 12:15am 
the next and continued working on the assignment until 3:13 am 9/10/2022.
On 9/10/2022 I continued working from 11am until 3:20pm with few mini breaks in between.

To Complete this StartUp Company Benifits project I've expected to complete the project within the most 3 days in total of 8 hours. In total I took 10 hours and 2 days 
to complete the assigment. I believe that it took longer than I've expected because I also rewatch the class to understand, read the class book and used google to
watch videos and learn more about coding in C#. I also took few breaks because I have kids. Next time, I will try to organize myself better with home responsabilities 
and rewatch the classes ahead of time and ask questions when it's needed. 
 */

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Moms_Talk_Crypto_Company_Benefits
{
    public partial class Form1 : Form
    {
       
        int die;
       

        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            MessageBox.Show("Welcome To Moms Talk Crypto Company Benefits Page");
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void CheckBonusbutton1_Click(object sender, EventArgs e)
        {
            decimal calcula_percentage = (Convert.ToDecimal(comboBox1.Text) / 100) * Convert.ToDecimal(textBox1.Text);
            textBox2.Text = (decimal.Parse(textBox1.Text) + calcula_percentage).ToString();
            {
            
            }



        }

        private void VacationDaysbutton1_Click(object sender, EventArgs e)
        {
            DateTime startdate = dobdateTimePicker1.Value;
            DateTime Enddate = dateTimePicker2.Value;
            textBox3.Text = CalcAge(startdate, Enddate).ToString();
            }
        public long CalcAge(System.DateTime StartDate, System.DateTime EndDate)
        {
            long age = 0;
            System.TimeSpan ts = new TimeSpan(EndDate.Ticks - StartDate.Ticks);
            age = (long)(ts.Days / 365);

            return age; 
        }
        private void button1_Click_1(object sender, EventArgs e)
        {
            Random random = new Random();
            die = random.Next(1, 10);
            MessageBox.Show("Extra Vacation Days =" + die);
            die++; //SC equivalent to die = die +1;
            MessageBox.Show("Bonus JACKPOT =" + die);
            die = die + 8;






        }

        private void Salarylabel1_Click(object sender, EventArgs e)
        {

        }

        private void FindOutBonuslabel1_Click(object sender, EventArgs e)
        {

        }

        private void comboBox1_SelectedIndexChanged(object sender, EventArgs e)
        {

        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void label1_Click_1(object sender, EventArgs e)
        {

        }

        private void dobdateTimePicker1_ValueChanged(object sender, EventArgs e)
        {

        }

        private void EnterYourAgelabel1_Click(object sender, EventArgs e)
        {

        }

        private void ExtraVacationlabel1_Click(object sender, EventArgs e)
        {

        }
    }

    
    }

