# Invoice Generator

This project contains scripts to generate invoices using a GUI and a template system. The main components are a GUI-based invoice generator (`main.py`) and a document generation script (`doc_gen.py`).

## Requirements

- Python 3.x
- `tkinter` library (usually included with Python)
- `docxtpl` library

You can install the required `docxtpl` library using pip:
```sh
pip install docxtpl
```

## Files

### main.py

This script creates a GUI application for generating invoices. It allows the user to input customer information and item details, and then generates an invoice document based on a template.

#### Features

- **Add Item**: Adds an item to the invoice with quantity, description, and unit price.
- **Generate Invoice**: Creates an invoice document with the provided details.
- **New Invoice**: Clears all input fields and the item list for a new invoice.

#### Usage

Run the script:
```sh
python main.py
```

The GUI will open, allowing you to enter the invoice details.

### doc_gen.py

This script demonstrates how to generate an invoice document using a predefined template and a list of items.

#### Features

- Loads a DOCX template.
- Renders the template with provided invoice data.
- Saves the generated invoice.

#### Usage

Ensure you have an `invoice_template.docx` in the same directory or specify the correct path in the script.

Run the script:
```sh
python doc_gen.py
```

## Configuration

Make sure to have a DOCX template for your invoices. The template should have placeholders that match the keys in the `render` method, such as `name`, `phone`, `invoice_list`, `subtotal`, `salestax`, and `total`.

## Example

The following is an example of how to use the GUI:

1. Run `main.py` to open the GUI.
2. Enter the customer's first name, last name, and phone number.
3. Add items to the invoice by specifying quantity, description, and unit price, then click "Add item".
4. Click "Generate Invoice" to create and save the invoice document.
5. Contact(kdkrish495@gmail.com).
6. To start a new invoice, click "New Invoice".
