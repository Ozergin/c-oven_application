namespace pasta_pisirme_prpject
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void progressBar1_Click(object sender, EventArgs e)
        {

        }

        private void timer1_Tick(object sender, EventArgs e)
        {
            progressBar1.Value += 10;
            if (progressBar1.Value % 20 == 0)
            {
                label1.BackColor = Color.White;
            }
            if (progressBar1.Value % 20 == 10)
            {
                label1.BackColor = Color.Red;
            }
            if (progressBar1.Value == 100)
            {
                timer1.Stop();
            }
            if (progressBar1.Value == 100)
            {
                timer1.Stop();
                timer2.Start();

            }
        }

        private void timer2_Tick(object sender, EventArgs e)
        {
            progressBar2.Value += 10;
            if (progressBar2.Value % 20 == 0)
            {
                label2.BackColor = Color.White;
            }
            if (progressBar2.Value % 20 == 10)
            {
                label2.BackColor = Color.Red;
            }
            if (progressBar2.Value == 100)
            {
                timer2.Stop();
            }
            if (progressBar2.Value == 100)
            {
                timer2.Stop();
                timer3.Start();
            }

        }

        private void timer3_Tick(object sender, EventArgs e)
        {
            progressBar3.Value += 10;
            if (progressBar3.Value % 20 == 0)
            {
                label3.BackColor = Color.White;
            }
            if (progressBar3.Value % 20 == 10)
            {
                label3.BackColor = Color.Red;
            }
            if (progressBar3.Value == 100)
            {
                timer3.Stop();
                timer4.Start();
            }

        }

        private void timer4_Tick(object sender, EventArgs e)
        {
            progressBar4.Value += 10;
            if(progressBar4.Value % 20 == 0)
            {
                label4.BackColor = Color.White;
            }
            if(progressBar4.Value %20 == 10)
            {
                label4.BackColor = Color.Red;
            }
            if(progressBar4.Value==100)
            {
                timer4.Stop();
                MessageBox.Show("pastanız hazır");
            }
        }
    }
}
