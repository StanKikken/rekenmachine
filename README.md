# rekenmachine
spreek eigenlijk wel voor zich





SOURCECODE


using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace reken
{
    public partial class Form1 : Form
    {
        string input =string.Empty;
        string op1 = string.Empty;
        string op2 = string.Empty;
        char operation;
        double result = 0.0;

        public Form1()
        {
            InitializeComponent();
        }

        private void label1_Click(object sender, EventArgs e)
        {

        }

        private void button_0_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "0";
            this.textBox1.Text += input;
        }

        private void button_dot_Click(object sender, EventArgs e)
        {
            input += ".";
        }

        private void button_equals_Click(object sender, EventArgs e)
        {
            op2 = input;
            double num1, num2;
            double.TryParse(op1, out num1);
            double.TryParse(op2, out num2);

            if (operation == '+')
            {
                result = num1 + num2;
                textBox1.Text = result.ToString();
            }
            else if (operation == '-')
            {
                result = num1 - num2;
                textBox1.Text = result.ToString();
            }
            else if (operation == '*')
            {
                result = num1 * num2;
                textBox1.Text = result.ToString();
            }
            else if (operation == '/')
            {
                if (num2 != 0)
                {
                    result = num1 / num2;
                    textBox1.Text = result.ToString();
                }
                else
                {
                    textBox1.Text = "DIV/Zero!";
                }
            }
        }

        private void button_plus_Click(object sender, EventArgs e)
        {
            op1 = input;
            operation = '+';
            input = string.Empty;
        }

        private void button_1_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "1";
            this.textBox1.Text += input;
        }

        private void button_2_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "2";
            this.textBox1.Text += input;
        }

        private void button_3_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "3";
            this.textBox1.Text += input;
        }

        private void button_minus_Click(object sender, EventArgs e)
        {
            op1 = input;
            operation = '-';
            input = string.Empty;
        }

        private void button_4_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "4";
            this.textBox1.Text += input;
        }

        private void button_5_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "5";
            this.textBox1.Text += input;
        }

        private void button12_Click(object sender, EventArgs e)
            //6
        {
            this.textBox1.Text = " ";
            input += "6";
            this.textBox1.Text += input;
        }

        private void button_x_Click(object sender, EventArgs e)
        {
            op1 = input;
            operation = '*';
            input = string.Empty;
        }

        private void button_7_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "7";
            this.textBox1.Text += input;
        }

        private void button_8_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "8";
            this.textBox1.Text += input;
        }

        private void button_9_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = " ";
            input += "9";
            this.textBox1.Text += input;
        }

        private void button_divide_Click(object sender, EventArgs e)
        {
            op1 = input;
            operation = '/';
            input = string.Empty;
        }

        private void button_backspace_Click(object sender, EventArgs e)
        {

        }

        private void button_clear_Click(object sender, EventArgs e)
        {
            this.textBox1.Text = "";
            this.input = string.Empty;
            this.op1 = string.Empty;
            this.op2 = string.Empty;
        }

        private void button_procent_Click(object sender, EventArgs e)
        {
            op1 = input;
            operation = '%';
            input = string.Empty;
        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        {

        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }
    }
}
