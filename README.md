# ResellerOS
ResellerOS

ResellerOS is a simple, beginner-friendly profit tracker for app resellers and anyone who buys and sells items for profit. It is written in Python with Streamlit, and the whole project lives in a single file, app.py, so it’s easy to read, run, and customize.

The app answers the questions every reseller cares about: How much have I actually made? Which categories are worth my time? Instead of juggling messy spreadsheets, you get a clean web interface that does the math for you.

Key features
Quick item entry: A form records the item name, category, buy price, sell price, date, and whether it has sold.
Inventory management: Every item appears in a table, with a delete button to remove mistakes in one click.
Dashboard: See your total profit, average margin percentage, and best-performing category at a glance.
Visual insights: A bar chart shows profit by category, so you can spot winners and losers instantly.
Persistent storage: Data is saved in a local SQLite database, so your records are still there after you close the app.
How it works

Profit and margin are calculated only for items marked as sold, so unsold stock never inflates your numbers. Margin is profit divided by sell price. Built-in validation stops you from saving items with an empty name or category, or sold items with no sell price.

Tech stack
Python 3.9+
Streamlit (user interface)
pandas (calculations)
SQLite (storage)
Getting started

Install the dependencies:

pip install -r requirements.txt

Then launch the app:

streamlit run app.py

Your browser will open automatically at http://localhost:8501.

Who is it for?

ResellerOS suits learners who want a practical first Python project, and small-scale resellers who want a lightweight tool they fully control. Fork it, tweak it, and make it your own.
