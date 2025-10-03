# 📋 Toba Welder - Quotation System

## 🎯 What is This?

This is a complete quotation management system designed for  **Toba Welder** , a welding, pergola, decking, and fencing service business. The system helps you create professional quotations, manage customer information, track pricing, and generate PDF documents - all running directly in your web browser with no server required.

## 🎥 Video Tutorial

Watch the complete video tutorial below to learn how to use the system:
<video width="100%" controls>
  <source src="https://drive.google.com/uc?export=download&id=1KUg8Lp9BwED_XBDgcjfXrLXgH2haJVl9" type="video/mp4">
  Your browser does not support the video tag.
</video>


---

## 🖥️ System Overview

### Three Main Screens

1. **Form Section** - Where you input quotation details
2. **Preview Section** - Shows your quotation before saving/downloading
3. **History Section** - Displays all saved quotations

### What Can You Do?

✅ **Create Quotations** - Generate professional quotes with company branding

✅ **Add Multiple Items** - List services, materials, and pricing

✅ **Auto-Calculate** - Automatic subtotal, GST (10%), and grand total

✅ **Preview in Real-Time** - See exactly how your quotation looks

✅ **Save to History** - Store up to 100 quotations locally

✅ **Download PDF** - Generate compact, professional PDF files

✅ **Print** - Print directly from browser

✅ **Edit Existing** - Copy and modify previous quotations

✅ **Export/Import** - Backup and restore your data

---

## 📝 How to Use

### Step 1: Creating a New Quotation

1. **Quote Number** is automatically generated based on the date:
   * Format: `YYYY/MM/DD/Number`
   * Example: `2025/10/04/001`
   * You only need to enter the last number
   * **Important:** Must be unique (system will warn you if it exists)
2. **Select Date** - Defaults to today, but you can change it
3. **Enter Customer Information:**
   * Customer Name (required)
   * Customer Address (required)
   * Phone (optional)
   * Email (optional)

### Step 2: Adding Items/Services

The items section starts with one row. For each item:

1. **Description** - What service/material (e.g., "Gate welding", "Steel fabrication")
2. **Quantity** - How many units
3. **Price** - Cost per unit in dollars
4. **Total** - Auto-calculated (Qty × Price)

**Actions:**

* Click **"➕ Add Item"** to add more rows
* Click **"✕ Delete"** to remove a row (must keep at least one)
* Totals update automatically as you type

### Step 3: Additional Information

* **Notes** (optional) - Payment terms, special instructions, warranty info, etc.

### Step 4: Generate Preview

Click **"⚡ Generate Quotation"** button

The system will:

* Validate all required fields
* Check for duplicate quote numbers
* Calculate subtotal, GST (10%), and total
* Show preview on the right side (or below on mobile)

### Step 5: Save, Download, or Print

**From Generated Preview:**

* **💾 Save** - Stores to local history
* **📥 Download PDF** - Creates compact, professional PDF
* **🖨️ Print** - Opens print dialog

**From History View:**

* **👁️ View** - Opens read-only preview
* **✏️ Edit** - Copies data as new quotation (change quote number)
* **🗑️ Delete** - Removes from history

---

## 💾 How Data is Saved

### Local Storage System

All data is saved in your browser's  **localStorage** :

* No server required
* No internet connection needed after initial load
* Data persists until you clear browser data
* Maximum 100 quotations stored (oldest deleted automatically)

### Important Notes

⚠️ **Data is tied to your browser**

* Different browsers = different data
* Incognito/Private mode = data lost when closed
* Clearing browser data = data lost

✅ **Backup Your Data**

Use **Export Data** button regularly to create backup files

### Quote Number Rules

* Must follow format: `YYYY/MM/DD/###`
* Must be unique across all saved quotations
* System auto-generates the prefix based on date
* You enter the suffix number (001, 002, etc.)
* When editing from history, you must change the number

---

## 🔧 Key Features Explained

### Automatic Calculations

* **Item Total** = Quantity × Price
* **Subtotal** = Sum of all item totals
* **GST** = Subtotal × 10%
* **Grand Total** = Subtotal + GST

### PDF Generation

The system creates compact, professional PDFs optimized for printing:

* A6 size (half of A4)
* Includes company logo and branding
* All customer and item details
* Payment information
* Digital signature section
* High-quality output

### Preview Modes

Two viewing contexts:

1. **Generate Mode** (new quotations)
   * Shows: Save, Download PDF, Print buttons
2. **View Mode** (from history)
   * Shows: Edit, Download PDF, Print buttons

### Export/Import System

**Export:**

* Creates `.json` backup file
* Filename includes timestamp
* Contains all quotation history

**Import:**

* Restores from `.json` file
* Replaces current history (be careful!)
* Validates file format

---

## 📊 History Management

### What's Stored

Each quotation includes:

* Quote number
* Date
* Customer name and address
* Contact details (phone/email)
* All items with pricing
* Notes
* Calculated totals
* Timestamp

### History Table Columns

* **Quote No.** - Unique identifier
* **Date** - Quotation date
* **Customer** - Customer name
* **Total** - Grand total including GST
* **Actions** - View, Edit, Delete buttons

### Limits

* Maximum: 100 quotations
* When full: Oldest quotation deleted automatically
* Solution: Export data regularly

---

## 🎨 Design Features

### Responsive Layout

* **Desktop:** Form and preview side-by-side
* **Tablet:** Single column with toggle
* **Mobile:** Optimized vertical layout

### Visual Feedback

* ✅ Success messages (green)
* ⚠️ Error messages (red)
* Animated transitions
* Hover effects on buttons
* Auto-scrolling to relevant sections

### Branding

* Company logo displayed
* Orange/blue color scheme
* Professional formatting
* Consistent typography

---

## ⚡ Quick Tips

1. **Before Starting:** Set the date first to get correct quote number prefix
2. **Duplicate Protection:** System prevents saving duplicate quote numbers
3. **Editing:** Always change the quote number when editing from history
4. **Backup:** Export your data weekly to prevent loss
5. **Printing:** Use browser's print function (Ctrl+P / Cmd+P)
6. **Mobile Use:** Rotate to landscape for better item table viewing
7. **Calculator:** System handles all math - just enter quantities and prices
8. **Notes Field:** Great for payment terms like "50% deposit required"

---

## 🛠️ Technical Details

### Browser Compatibility

Works on modern browsers:

* Chrome/Edge (recommended)
* Firefox
* Safari
* Opera

### Storage Capacity

* Average quotation: ~2KB
* 100 quotations: ~200KB
* Well within localStorage limits (5-10MB)

### Libraries Used

* **html2canvas** - Converts HTML to image for PDF
* **jsPDF** - Generates PDF documents
* Pure JavaScript (no frameworks)
* CSS Grid & Flexbox for layout

### No Installation Required

Just open `quotation.html` in your browser and start using!

---

## 🚨 Troubleshooting

**PDF Won't Generate?**

* Refresh the page
* Check browser console for errors
* Try different browser

**Quote Number Already Exists?**

* Check history table for duplicate
* Change the number suffix
* Delete old quotation if it's a mistake

**Data Disappeared?**

* Did you clear browser data?
* Check if you're in incognito mode
* Import from backup if available

**Items Not Calculating?**

* Enter valid numbers only
* Don't use currency symbols in inputs
* Check quantity is at least 1

---

## 📞 Company Information

**Toba Welder**

49 Bloomfield Avenue, Maribyrnong 3032

ABN: 49280241868

Phone: 0431509279

Email: samosirbram1974@gmail.com

---

## 📄 File Structure

```
quotation.html          # Main application file
logo.png               # Company logo (optional)
TUTORIAL.mp4          # Video tutorial
README.md             # This file
```

---

## ✨ Best Practices

1. **Regular Backups** - Export data at least weekly
2. **Consistent Numbering** - Use sequential numbers (001, 002, 003...)
3. **Complete Information** - Fill all customer details for professional look
4. **Clear Descriptions** - Be specific in item descriptions
5. **Review Before Saving** - Check preview carefully
6. **Professional Notes** - Add payment terms and warranties

---

## 🎓 Getting Started Checklist

* [ ] Open `quotation.html` in your browser
* [ ] Watch `TUTORIAL.mp4` for complete guide
* [ ] Create your first test quotation
* [ ] Download the PDF to see output quality
* [ ] Save to history
* [ ] Practice editing from history
* [ ] Export your data as backup
* [ ] Bookmark the file for easy access

---

**Ready to create professional quotations in minutes!** 🚀

