I want to make a program that will scrape craigslist and alert me when new apartments under 500 are available.
With this program I want it to:
  - Make the program sort out junk postings
  - sort out duplicate postings
  - when a new place under 500 is posted I want it to email me
  - save apartments to an excel document and delete postings after they are removed from craigslist but still make sure I am not shown apartments I have seen before



References:
- Python Features
  - [`__main__`](https://docs.python.org/3/library/__main__.html#idiomatic-usage) [StackOverflow explanation](https://stackoverflow.com/questions/419163/what-does-if-name-main-do)
  - [Type hints](https://docs.python.org/3/library/typing.html)
  - [Generators](https://realpython.com/introduction-to-python-generators/)
  - [Walrus operator](https://realpython.com/python-walrus-operator/)
  - [Regular expression operations](https://docs.python.org/3/library/re.html) (regex)
    - [Greedy versus Non-Greedy](https://docs.python.org/3/howto/regex.html#greedy-versus-non-greedy)
    - [Named Groups](https://docs.python.org/3/howto/regex.html#non-capturing-and-named-groups)
    - Examples used
      - [`LOCATION_REGEX`](https://pythex.org/?regex=%5C((%3FP%3Cinner%3E.*%3F)%5C)&test_string=%20%20%20asdf%20%20%20(%20%20location%20)%20asdf&ignorecase=1&multiline=0&dotall=0&verbose=0)
      - [`BED_REGEX`](https://pythex.org/?regex=(%3FP%3Cbr%3E%5Cd%2B)br&test_string=%242%2C064%2F%203br%20-%201362ft2%20-%20&ignorecase=1&multiline=0&dotall=0&verbose=0)
- CSS Selectors
  - [Select by ID](https://www.w3schools.com/csSref/sel_id.asp)
  - [Select by class](https://www.w3schools.com/cssref/sel_class.asp)
  - [Select by attribute begin](https://www.w3schools.com/cssref/sel_attr_begin.asp)
- openpyxl
  - [`load_workbook`](https://openpyxl.readthedocs.io/en/stable/api/openpyxl.reader.excel.html?highlight=load_workbook#openpyxl.reader.excel.load_workbook)
  - [`Worksheet.iter_rows`](https://openpyxl.readthedocs.io/en/stable/api/openpyxl.worksheet.worksheet.html#openpyxl.worksheet.worksheet.Worksheet.iter_rows)
  