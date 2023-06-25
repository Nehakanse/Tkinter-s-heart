# Tkinter-s-heart
This code provides a simple and concise way to generate a heart shape using Tkinter, allowing for further customization and integration into larger graphical applications. Tkinter's versatility makes it a suitable choice for developing interactive GUIs in Python.
import tkinter as tk

root = tk.Tk()
canvas = tk.Canvas(root, width=200, height=200)
canvas.pack()

# Coordinates for the heart shape
x0, y0 = 100, 100
scale = 40

# Draw the heart shape
canvas.create_polygon(x0, y0 - 2*scale, x0 - scale, y0 - 3*scale, x0 - 2*scale, y0 - scale,
                      x0 - 2*scale, y0, x0, y0 + 2*scale, x0 + 2*scale, y0, x0 + 2*scale,
                      y0 - scale, x0 + scale, y0 - 3*scale, fill='red', outline='')

root.mainloop()

