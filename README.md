# Browse
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Diagnostics;
using System.IO;
using System.Windows.Forms;

namespace Bagaev_web
{
    public partial class Form1 : Form
    {

        public Form1()

        {
            InitializeComponent();
        }
        public void OnKeyPress(object sender, System.Windows.Forms.KeyEventArgs e)
        {
            if (e.KeyCode == Keys.Enter)
            {
                comboBox1.SelectedItem.ToString();
                
            }

        }
       
        private void button1_Click_1(object sender, EventArgs e)
        {
            webBrowser1.Navigate("SMTP://" + comboBox1.Text);
            webBrowser1.Navigate("https://" + comboBox1.Text);
            webBrowser1.Navigate("http://" + comboBox1.Text);
            comboBox1.Items.Add("yandex.ru");
            comboBox1.Items.Add("google.ru");
            comboBox1.Items.Add("");
            comboBox1.Items.Add("mail.yandex.ru/");
            comboBox1.Items.Add("mail.ru");
            comboBox1.Items.Add("vk.com");
            comboBox1.Items.Add("facebook.com");
            comboBox1.Items.Add("rutracker.org");
            comboBox1.Items.Add("free.drweb.ru/download+cureit+free/?lng=ru");
            comboBox1.Items.Add("ccleaner.org.ua/download/");
            comboBox1.Items.Add("teamviewer.com/ru/download/windows/");
            
        }

   

        private void button2_Click (object sender, EventArgs e)
            {
                Close();
            }

        private void button_3Click (object sender, EventArgs e)
        {
                    
                webBrowser1.Navigate("file:\\" + comboBox2.Text);
                comboBox2.Items.Add("\\C:\\");
                comboBox2.Items.Add("\\D:\\");
                comboBox2.Items.Add("\\E:\\");
                comboBox2.Items.Add("\\G:\\");
                comboBox2.Items.Add("\\I:\\");
                comboBox2.Items.Add("\\K:\\");
                comboBox2.Items.Add("\\L:\\");
                comboBox2.Items.Add("\\M:\\");
                comboBox2.Items.Add("\\H:\\");
                comboBox2.Items.Add("\\F:\\");
                comboBox2.Items.Add("\\A:\\");
                comboBox2.Items.Add("\\S:\\");
                comboBox2.Items.Add("\\W:\\");
                comboBox2.Items.Add("\\R:\\");
                comboBox2.Items.Add("\\C:\\ProgramData\\Microsoft\\Windows\\Start Menu\\Programs\\Accessories\\");
                comboBox2.Items.Add("\\C:\\ProgramData\\Microsoft\\Windows\\Start Menu\\Programs\\Microsoft Office\\");
                comboBox2.Items.Add("\\C:\\ProgramData\\Microsoft\\Windows\\Start Menu\\Programs\\Administrative Tools\\");


            }

       

        private void button4_Click (object sender, EventArgs e)
            {
                System.Diagnostics.Process.Start("Bagaev_web.exe");

            }

        private void button5_Click (object sender, EventArgs e)
            {
                webBrowser1.Navigate(webBrowser1.Url);
            }

        private void button6_Click (object sender, EventArgs e)
            {
                webBrowser1.GoBack();
            }

        private void button7_Click (object sender, EventArgs e)
            {
                webBrowser1.GoForward();
            }

        private void button8_Click (object sender, EventArgs e)
        {
            
            webBrowser1.GoSearch();

        }

       

        
    }


    }

         How can I run this program automatically instead of a standard browser?
