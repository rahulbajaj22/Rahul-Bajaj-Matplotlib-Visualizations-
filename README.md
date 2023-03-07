# Rahul-Bajaj-Matplotlib-Visualizations-
# These are my visualizations I've created using matplotlib software program. 


csd_dataset = pd.read_csv('company_sales_data.csv')
month_number = csd_dataset['month_number'].tolist()
facecream_salesdata = csd_dataset['facecream'].tolist()
facewash_salesdata = csd_dataset['facewash'].tolist()
toothpaste_salesdata = csd_dataset['toothpaste'].tolist()
bathingsoap_salesdata = csd_dataset['bathingsoap'].tolist()
shampoo_salesdata = csd_dataset['shampoo'].tolist()
moisturizer_salesdata = csd_dataset['moisturizer'].tolist()

plt.plot([], [], label = 'Facecream', color = 'black')
plt.plot([], [], label = 'Facewash', color = 'red')
plt.plot([], [], label = 'Toothpaste', color = 'blue')
plt.plot([], [], label = 'Toothpaste', color = 'orange')
plt.plot([], [], label = 'Toothpaste', color = 'green')
plt.plot([], [], label = 'Toothpaste', color = 'white')

plt.stackplot(month_number, facecream_salesdata, facewash_salesdata, toothpaste_salesdata, bathingsoap_salesdata,
shampoo_salesdata, moisturizer_salesdata, colors = ['black', 'red', 'blue', 'orange', 'green', 'white'])

plt.legend(loc = 'upper left')
plt.xlabel('Month Number')
plt.ylabel('Sales units in numbers')
plt.title('All product sales data using stack plot!')
plt.show()
