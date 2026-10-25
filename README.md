# Hydrophobicity Coloring Tool

Colors in structural depictions of proteins are critical for effective
communication. During my PhD, I became unhappy with the default colors
in ChimeraX and the colors of color_h (https://pymolwiki.org/Color_h) for PyMol. 
I wrote my own script in Python to take the same scale as color_h with fully
customizable colors. At the end of my PhD, I asked Claude to translate it into
HTML to make a web tool. This is the result:

A browser-based tool that generates ChimeraX and PyMOL scripts to color protein
surfaces by residue hydrophobicity, using a user-controlled two-color gradient.

**[Launch the tool](https://<username>.github.io/<repo>/)**

## Features

- Provides scripts for both **ChimeraX** and **PyMOL**
- Choose your own hydrophilic and hydrophobic colors.
- Colors fade to medium gray (`#808080`) at the zero point of the scale.
- Live gradient preview and one-click copy.

## How to use

1. Open the tool and choose ChimeraX or PyMOL.
2. Pick your hydrophilic and hydrophobic colors.
3. (Optional) Enter a PDB ID to include an open/fetch command.
4. Click **Copy** and paste the script into the ChimeraX or PyMOL command line.

## Scale

Residue values come from the Eisenberg normalized consensus hydrophobicity
scale (Eisenberg, 1984). Each residue's color is interpolated between gray and
your chosen color.

## Running locally

No install needed. Download `index.html` and open it in a browser.

## Credits

Created by Dante M. Avalos, inspired by the `color_h` script.
