# SWAPI Project
![SWAPI](png/Image.jpg)
In a galaxy far, far away, the star wars APIs were raging... Wait! Something's not right here, what are these APIs? API stands for Application Programming Interface, or in Russian, it means the application's program interface. Usually, when data engineers talk about API, they mean a website that can be accessed according to certain rules and will return a predetermined standard response. SWAPI, or Star Wars API, is just such an example. It stores information about characters, spaceships, planets, and other objects related to the "Star Wars" universe.

---
Script Operation
--
**Importing requests:** The requests library is used for sending HTTP requests.
**From the pathlib module:** The Path class is utilized to work with files and directories.
**The APIRequester Class:** Initializes an object with a base URL (base_url), so that all requests are performed relative to this address.The get() method sends GET requests to the specified path (tail_url) and returns the server's response. If an error occurs, it is handled through a try/except block.
**Subclass SWRequester:** This class inherits from APIRequester. It implements additional methods for working with the Star Wars API.

The get_sw_categories() method queries the root path of the API and extracts available categories (e.g., "films," "people," "planets").
The get_sw_info() method queries a specific category and returns its content.
Function save_sw_data():
A folder named data is created to store files.
For each category, a request is made to the API, and the result is saved into separate text files in this folder.
In summary, this script interacts with the Star Wars API, retrieves information by category, and saves the data into individual files.
