# Matplotlib

Line Plot

import matplotlib.pyplot as plt

### Data
x = [1, 2, 3, 4]
y = [10, 20, 25, 30]

### Create the plot
plt.plot(x, y)

### Show the plot
plt.show()
Scatter Plot


import matplotlib.pyplot as plt

### Data
x = [1, 2, 3, 4]
y = [10, 20, 25, 30]

### Create the plot
plt.scatter(x, y)

### Show the plot
plt.show()
Bar Plot


import matplotlib.pyplot as plt

### Data
x = ['Cat', 'Dog', 'Fish']
y = [10, 20, 15]

### Create the plot
plt.bar(x, y)

### Show the plot
plt.show()
Histogram


import matplotlib.pyplot as plt

# Data
x = [10, 20, 25, 30, 35, 40, 45, 50]

# Create the plot
plt.hist(x, bins=4)

# Show the plot
plt.show()
Pie Chart


import matplotlib.pyplot as plt

# Data
labels = ['Cat', 'Dog', 'Fish']
sizes = [10, 20, 15]

# Create the plot
plt.pie(sizes, labels=labels)

# Show the plot
plt.show()



# Seaborn
