# DashBoard 
> Modern Flat UI Design Dashboard in material design application in c# windows.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [What I Did By Myself](#what-i-did-by-myself)
* [Project Status](#project-status)
* [Sources](#sources)

## General Information
- I made a simple design of a Dashboard to learn it.
- This is a window with several options to click.

## Technologies Used
.Net Framework 4.7.2

## What I Did By Myself
- All graphics and icons.
- I found a bug
  In the tutorial in code 
   public Form1()
        {
            InitializeComponent();
            Region = System.Drawing.Region.FromHrgn(CreateRoundRectRgn(0, 0, Width, Height, 25, 25));

            pnlNav.Height = btnDashboard.Height;
            pnlNav.Top = btnDashboard.Top;
            pnlNav.Left = btnDashboard.Left;
            btnDashboard.BackColor = Color.FromArgb(24, 30, 54); //first problem. Color numbers was wrong. 
                                                                 //This one 46, 51, 73, so DashBoard button all time lighting by this color.
            lblTitle.Text = "Dashboard";
            this.PnlFormLeader.Controls.Clear();
            frmDashboard FrmDashboard_Vrb = new frmDashboard() { Dock = DockStyle.Fill, TopLevel = false, TopMost = true };
            FrmDashboard_Vrb.FormBorderStyle = FormBorderStyle.None;
            this.PnlFormLeader.Controls.Add(FrmDashboard_Vrb);
            FrmDashboard_Vrb.Show();

        }      


## Project Status
Project is: _in progress_ (I have a few problems to fix).

## Sources
This project was based on [this tutorial part 1](https://www.youtube.com/watch?v=vYDyGxoq9JU&list=WL&index=10).
[Tutorial part 2](https://www.youtube.com/watch?v=3ox-6NFAt8I).
