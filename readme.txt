using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp1
{
    public partial class Form1 : Form
    {
        Random rnd;
        public Form1()
        {
            InitializeComponent();
            rnd = new Random();
        }

        private void button1_Click(object sender, EventArgs e)
        {

        }

        private void button1_Click_1(object sender, EventArgs e)
        {

        }

        private void label3_Click(object sender, EventArgs e)
        {

        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void button3_Click(object sender, EventArgs e)

        {
            try
            {
                int num1, num2;
                if (textBox1.Text != "") {
                    num1 = int.Parse(textBox1.Text); }
                else num1 = 0;
                if (textBox2.Text != "")
                {
                    num2 = int.Parse(textBox2.Text);
                }
                else num2 = 0;
                int result = num1 + num2;
                textBox3.Text = result.ToString();
            }
            catch(Exception ex)
            {
                MessageBox.Show(ex.Message);
            }
        }

        private void button4_Click(object sender, EventArgs e)
        {
            try
            {
                int num1, num2;
                if (textBox1.Text != "")
                {
                    num1 = int.Parse(textBox1.Text);
                }
                else num1 = 0;
                if (textBox2.Text != "")
                {
                    num2 = int.Parse(textBox2.Text);
                }
                else num2 = 0;
                int result = num1 * num2;
                textBox3.Text = result.ToString();
            }
            catch (Exception ex)
            {
                MessageBox.Show(ex.Message);
            }
        }

        private void button5_Click(object sender, EventArgs e)
        {
            try
            {
                int num1, num2;
                if (textBox1.Text != "")
                {
                    num1 = int.Parse(textBox1.Text);
                }
                else num1 = 0;
                if (textBox2.Text != "")
                {
                    num2 = int.Parse(textBox2.Text);
                }
                else num2 = 1;
                int result = num1 % num2;
                textBox3.Text = result.ToString();
            }
            catch (Exception ex)
            {
                MessageBox.Show(ex.Message);
            }
        }

        private void textBox3_TextChanged(object sender, EventArgs e)
        {

        }

        private void button1_Click_2(object sender, EventArgs e)
        {
            textBox1.Text = rnd.Next(0, 10000).ToString();

        }

        private void button2_Click(object sender, EventArgs e)
        {
            textBox2.Text = rnd.Next(0, 10000).ToString();
        }

        private void button6_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '1';
            
        }

        private void button13_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '8';
        }

        private void button7_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '2';
        }

        private void button8_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '3';
        }

        private void button9_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '4';
        }

        private void button10_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '5';
        }

        private void button11_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '6';
        }

        private void button12_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '7';
        }

        private void button14_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox1.Text.Length) && (textBox1.Text[cut] == '0'); cut++) ;
            textBox1.Text = textBox1.Text.Remove(0, cut) + '9';
        }

        private void button15_Click(object sender, EventArgs e)
        {
            bool q = true;
            foreach (char c in textBox1.Text)
                if (c != '0')
                    q = false;
            if ((textBox1.Text.Length == 0) || (!q))
                textBox1.Text += "0";
        }

        private void button25_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '1';
        }

        private void button24_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '2';
        }

        private void button23_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '3';
        }

        private void button22_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '4';
        }

        private void button21_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '5';
        }

        private void button20_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '6';
        }

        private void button19_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '7';
        }

        private void button18_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '8';
        }

        private void button17_Click(object sender, EventArgs e)
        {
            int cut = 0;
            for (; (cut < textBox2.Text.Length) && (textBox2.Text[cut] == '0'); cut++) ;
            textBox2.Text = textBox2.Text.Remove(0, cut) + '9';
        }

        private void button16_Click(object sender, EventArgs e)
        {
            bool q = true;
            foreach (char c in textBox2.Text)
                if (c != '0')
                    q = false;
            if ((textBox2.Text.Length == 0) || (!q))
                textBox2.Text += "0";
        }

        private void button26_Click(object sender, EventArgs e)
        {
            textBox2.Text = "";
        }

        private void button27_Click(object sender, EventArgs e)
        {
            textBox1.Text = "";
        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        {

        }
    }
}
