# Amazon_scrape_final
This Python script is designed to scrape product details from Amazon's search results pages. It extracts the following information for each product:

<ul>
        <li>Product Title</li>
        <li>Product Price</li>
        <li>Product Rating</li>
        <li>Number of User Reviews</li>
        <li>Product Availability</li>
</ul>

The data is then stored in a CSV file for easy analysis.

# Requirements

To run this script, you will need the following Python libraries:

<ul>
        <li><code>requests</code> (for making HTTP requests)</li>
        <li><code>beautifulsoup4</code> (for parsing HTML content)</li>
        <li><code>pandas</code> (for storing and manipulating the data)</li>
        <li><code>numpy</code> (for handling missing data)</li>
</ul>
You can install the required libraries using <code>pip</code>:
    <pre><code>pip install requests beautifulsoup4 pandas numpy</code></pre>

# How To Use 

<ol>
        <li><strong>Set the Target URL:</strong>
            <p>Modify the <code>URL</code> variable in the script to the Amazon search URL you want to scrape. The default is set to the search results page for "PlayStation 4".</p>
        </li>
        <li><strong>Set the User-Agent:</strong>
            <p>Add a valid User-Agent string in the <code>HEADERS</code> variable to avoid being blocked by Amazon's anti-scraping measures. You can find your User-Agent by inspecting the request headers in your browser’s developer tools.</p>
        </li>
        <li><strong>Run the Script:</strong>
            <p>After setting the correct URL and headers, you can run the script using:</p>
            <pre><code>python amazon_scraper.py</code></pre>
        </li>
        <li><strong>Output:</strong>
            <p>The script will output a CSV file (<code>amazon_data.csv</code>) that contains the product details for each item on the search results page.</p>
        </li>
    </ol>

# Disclaimer

This script is for educational purposes only. Web scraping Amazon may violate their terms of service, so use this script responsibly and consider using Amazon's official APIs for legitimate access to their data.
