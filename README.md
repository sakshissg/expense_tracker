# Group Expense Tracker

A simple yet powerful web-based expense tracker for splitting costs among friends. Perfect for group trips, shared meals, or any situation where multiple people need to split expenses fairly.

## 🌟 Features

- **Friend Management**: Easily add or remove friends from your group
- **Flexible Expense Tracking**: Record who paid and who participated in each expense
- **Smart Settlement Calculation**: Automatically calculates who owes what to whom
- **Optimized Transactions**: Minimizes the number of payments needed to settle up
- **Real-time Updates**: Instantly see balance changes as you add expenses
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **No Dependencies**: Pure HTML, CSS, and JavaScript - no frameworks required

## 🚀 Quick Start

1. **Download**: Save the HTML file to your computer
2. **Open**: Double-click the file or open it in any web browser
3. **Start Tracking**: Begin adding friends and expenses immediately

No installation, no setup, no internet connection required!

## 📱 How to Use

### Adding Friends
1. Type a friend's name in the "Add friend name" field
2. Click the "Add" button or press Enter
3. Remove friends by clicking the × next to their name (minimum 1 friend required)

### Recording Expenses
1. Click "Add Expense" to create a new expense entry
2. Fill in the details:
   - **Description**: What was the expense for (e.g., "Dinner", "Movie tickets")
   - **Amount**: Total cost of the expense
   - **Paid By**: Select who actually paid the money
   - **Participants**: Check the boxes for everyone who should share this cost
   - **Date**: When the expense occurred (defaults to today)
3. Click "Remove" to delete an expense if needed

### Understanding the Settlement
The app automatically calculates and displays:
- **Individual Balances**: How much each person is owed (+) or owes (-)
- **Settlement Instructions**: Exact payments needed to settle all debts
- **Total Summary**: Overall expense amount for the group

## 💡 Example Scenarios

### Scenario 1: Haircuts
- 3 friends go out, but only 2 get haircuts
- Friend A pays $60 for both haircuts
- **How to record**: Amount: $60, Paid by: Friend A, Participants: Friend A + Friend B only
- **Result**: Friends A and B each owe $30, Friend C owes nothing

### Scenario 2: Group Dinner
- All 3 friends have dinner together
- Friend B pays the $90 bill
- **How to record**: Amount: $90, Paid by: Friend B, Participants: All 3 friends
- **Result**: Friends A and C each owe Friend B $30

### Scenario 3: Multiple Expenses
After both expenses above:
- Friend A: Paid $60, owes $30 → Net: +$30 (owed $30)
- Friend B: Paid $90, owes $30 → Net: +$60 (owed $60)
- Friend C: Paid $0, owes $60 → Net: -$60 (owes $60)
- **Settlement**: Friend C pays $30 to Friend A and $30 to Friend B

## 🎯 Key Benefits

- **Fair Splitting**: Only pay for what you participated in
- **Simplified Settlement**: Minimizes the number of transactions needed
- **Transparent Calculation**: See exactly how amounts are calculated
- **Flexible Participation**: Not everyone needs to participate in every expense
- **Mobile Friendly**: Track expenses on the go
- **Privacy Focused**: All data stays in your browser - no cloud storage

## 🛠️ Technical Details

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Compatibility**: Works in all modern web browsers
- **Storage**: In-memory only (data resets when page is refreshed)
- **Dependencies**: None - completely self-contained
- **File Size**: ~15KB total


## 🎨 Features in Detail

### Smart Settlement Algorithm
The app uses an optimized debt settlement algorithm that:
1. Calculates each person's net balance (what they paid vs. what they owe)
2. Identifies creditors (people owed money) and debtors (people who owe money)
3. Creates the minimum number of transactions to settle all debts
4. Prioritizes larger amounts first for efficiency

### Responsive Design
- **Desktop**: Full-width layout with side-by-side sections
- **Tablet**: Stacked sections with comfortable spacing
- **Mobile**: Single-column layout optimized for touch interaction

### User Experience
- **Real-time Updates**: Calculations update immediately as you type
- **Visual Feedback**: Color-coded balances (green for owed, red for owing)
- **Error Prevention**: Form validation and sensible defaults
- **Intuitive Interface**: Clear labels and logical flow

## 📝 Data Persistence

**Important Note**: This app stores data in browser memory only. Data will be lost when:
- The page is refreshed
- The browser tab is closed
- The browser is restarted

For permanent storage, consider:
- Bookmarking the page and taking screenshots of results
- Copying settlement instructions to notes
- Using browser bookmarks to save the state

## 🔧 Customization

The app is designed to be easily customizable:

### Adding New Features
- Modify the `expenses` array structure to add new fields
- Update the `renderExpenses()` function to display new fields
- Extend the settlement calculation in `calculateSettlement()`

### Styling Changes
- All styles are in the `<style>` section of the HTML file
- Uses CSS custom properties for easy color scheme changes
- Responsive breakpoints can be adjusted in the media queries

### Functionality Extensions
- Add export functionality for settlement results
- Implement local storage for data persistence
- Add expense categories or tags
- Create printable reports

## 🤝 Use Cases

Perfect for:
- **Group Trips**: Hotels, meals, activities, transportation
- **Roommate Expenses**: Utilities, groceries, household items
- **Office Lunches**: Team meals and group orders
- **Social Events**: Party planning, group gifts, shared activities
- **Project Expenses**: Team supplies and shared resources

## 📋 Tips for Best Results

1. **Be Specific**: Use clear expense descriptions like "Pizza dinner at Mario's" instead of just "food"
2. **Check Participants**: Double-check who should be included in each expense
3. **Regular Updates**: Add expenses as they happen rather than trying to remember later
4. **Round Numbers**: Consider rounding to nearest dollar for easier settlement
5. **Screenshot Results**: Save settlement instructions before closing the browser

## 🆘 Troubleshooting

**Q: My data disappeared when I refreshed the page**
A: The app doesn't save data permanently. Consider taking screenshots of important settlement information.

**Q: The settlement seems wrong**
A: Verify that participants are correctly selected for each expense and amounts are accurate.

**Q: Can't remove a friend**
A: You need at least one friend in the group. Add another friend first, then remove the unwanted one.

**Q: Calculations don't add up**
A: Check that all expense amounts are entered correctly and participants are properly selected.

## 📄 License

This project is open source and available under the MIT License. Feel free to modify, distribute, and use for any purpose.

## 🙏 Acknowledgments

Created with modern web technologies and responsive design principles. Inspired by popular expense-splitting apps but designed to be simple, fast, and privacy-focused.

---

**Happy expense tracking!** 🎉

*For questions, suggestions, or contributions, feel free to reach out or modify the code to suit your needs.*
