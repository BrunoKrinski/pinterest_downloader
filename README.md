<h1>Pinterest Download Tools</h1>
<p>See details on: <a target="_blank" href="https://brunokrinski.github.io/pinterest-download-tools/">https://brunokrinski.github.io/pinterest-download-tools/</p>

<h1>Download:</h1>
<pre><code>git clone https://github.com/BrunoKrinski/pinterest-download-tools.git</code></pre>

<h1>Installation:</h1>

<h2>Step 1:</h2>
<pre><code>pip install -r requirements.txt</code></pre>

<h2>Step 2:</h2>
<ul>
    <li>Install the Firefox.</li>
    <li>Download <a target="_blank" href="https://github.com/mozilla/geckodriver/releases">Geckodriver</a> and put on your system path.</li>
</ul>

<h1>Usage:</h1>

<h2>Images Downloader:</h2>
<pre><code>python download_pinterest_images.py --email your_email@gmail.com --passwd your_password --link url_to_pinretest_folder</code></pre>
<pre><code>python download_pinterest_images.py --email your_email@gmail.com --passwd your_password --list list_of_url.txt</code></pre>
<p>The list of links must be a .txt file where each line in the file is a url to a pinterest folder.</p>

<h2>Find duplicates:</h2>
<pre><code>python find_duplicates.py --folder path_to_the_images_folder</code></pre>
<p>The duplicated images will be in a folder called duplicates</p>

<h2>Remove borders:</h2>
<pre><code>python remove_black_borders.py --folder path_to_the_images_folder</code></pre>
<pre><code>python remove_white_borders.py --folder path_to_the_images_folder</code></pre>
<p>Move the images you want to remove the borders to a separete folder first and make a backup copy.</p>

<h2>Image selector:</h2>
<pre><code>python image_selector.py --folder path_to_the_images_folder</code></pre>
<h3>List of actions:</h3>
<ul>
    <li>keys: 0, 1, 2, ..., 8, 9 - Move the image to a folder0, folder1, ..., folder9.</li>
    <li>key: s - Move the image to folder saved.</li>
    <li>key: d - Move the image to folder trash.</li>
    <li>key: n - Skip the current image.</li>
    <li>key: q - End the program.</li>
</ul>