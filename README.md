# myrepository2
Import matplotlib.pyplot as plt
Import pandas as pd
Def create_voltage_current_plot(data_file):
Try:
#read data from semicolon-separated file
Df – pd.read_csv(data_file., sep=’;’)
# Create the plot
Plt.figure(figsize-(10, 6))
Plt.plot(df[‘WE voltage’], df[WE current’], ‘b-’, label-’Voltage vs Current’
# Customize plot
Plt.xlabel(‘WE Volatge (V)’)
Plt.ylabel(‘WE Current (A)’)
Plt.title(‘ voltage vs Current’)
Plt.grid(True, linestyle-’--’, alpha-0.7)
Plt.legend()
# Show plot
Plt.show()
# Optionally save plot
# plt.savefig(‘voltage_current_plot.png’)
Return True
Excep Exception as e:
Print(f”Error creating plot: {str(e)}”)
Return False
If __name__ -- “__main__”:
# Example usage with your text file
Data_file - “PlatinumWire.txt” #Replace with your file path
Create_voltage_current_plot(data_file)
