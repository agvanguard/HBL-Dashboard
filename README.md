# Healthy Backlog Limits (HBL) Dashboard

A real-time dashboard to monitor team capacity and unassigned tickets across support teams.

## 📊 Overview

This dashboard displays the Healthy Backlog Limits (HBL) for various support teams and their current unassigned ticket counts. The unassigned ticket limit is set at **25% of the HBL**.

## 🚀 Live Dashboard

[View Live Dashboard](#) *(Add your deployed URL here after deployment)*

## 📁 Files in this Repository

- `dashboard.jsx` - React component for the dashboard
- `Healthy_Backlog_Limits_-_For_HBL_Dashboard.csv` - Data source file

## 📋 Data Columns

The dashboard displays the following information:
- **Subgroup** - Support category (e.g., Admin Support, Core Product Support)
- **Team** - Team name
- **HBL** - Healthy Backlog Limit (maximum ticket capacity)
- **Unassigned Tickets** - Current number of unassigned tickets

## 🔄 How to Update Data

1. Navigate to `Healthy_Backlog_Limits_-_For_HBL_Dashboard.csv` in this repository
2. Click the **pencil icon** (Edit this file)
3. Update the data following the CSV format:
   ```
   Subgroup,Team,Healthy Backlog Limit (HBL*),# of Unassigned Tickets
   Admin Support,Admin APJ,6,1
   Admin Support,Admin EMEA,10,2
   ```
4. Click **"Commit changes"**
5. Users can click the **"Refresh Data"** button on the dashboard to see the latest updates

## 💻 Local Development

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
   cd YOUR_REPO
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Update the CSV_URL in `dashboard.jsx` (line 11) to point to your GitHub raw file URL

4. Run the development server:
   ```bash
   npm start
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## 🌐 Deployment

### Deploy with Vercel (Recommended)

1. Sign up at [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. Import this GitHub repository
4. Click "Deploy"
5. Your dashboard will be live in minutes!

### Deploy with Netlify

1. Sign up at [netlify.com](https://netlify.com)
2. Click "Add new site" → "Import an existing project"
3. Connect to GitHub and select this repository
4. Click "Deploy site"

## 🔧 Configuration

To use this dashboard with your own data:

1. Fork or clone this repository
2. Replace the CSV file with your own data (keep the same format)
3. Update the `CSV_URL` in `dashboard.jsx`:
   ```javascript
   const CSV_URL = 'https://raw.githubusercontent.com/YOUR_USERNAME/YOUR_REPO/main/YOUR_CSV_FILE.csv';
   ```

## 📝 CSV Format

Maintain the following CSV structure:

```csv
Subgroup,Team,Healthy Backlog Limit (HBL*),# of Unassigned Tickets
Subgroup Name,Team Name,100,25
```

- Column 1: Subgroup name
- Column 2: Team name
- Column 3: HBL value (integer)
- Column 4: Unassigned ticket count (integer)

## 📞 Support

For questions or issues, please [open an issue](https://github.com/YOUR_USERNAME/YOUR_REPO/issues) in this repository.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Note:** Remember to keep your CSV data updated regularly for accurate dashboard metrics. The unassigned ticket limit is 25% of the HBL.
