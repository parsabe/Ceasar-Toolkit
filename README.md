
<img src="logo.png" width="1080" height="540">
<h1>Ceasar Toolkit</h1>

<p><strong>Ceasar Cipher Toolkit</strong> is a free, open-source CLI framework for encoding and decoding files using the classic Ceasar cipher. It also includes powerful tools to encrypt PDFs and folders — without compressing or modifying original file contents.</p>

<p><strong>No command-line arguments required</strong> — just run and go. The interactive menu handles everything.</p>



<h2> Features</h2>

<ul>
  <li>Interactive menu-driven interface</li>
  <li>Ceasar cipher encode/decode with header-based shift tracking</li>
  <li>PDF file encryption and decryption with password</li>
  <li>Folder encryption using <code>encfs</code> (no zipping or renaming)</li>
  <li>Animated loading spinners for all actions</li>
  <li>Colorized success/error messages with <code>colorama</code></li>
</ul>

<h2> Example Use</h2>

<pre><code>python main.py</code></pre>

<p>Then choose one of the options:</p>
<pre><code>
1. Ceasar Encode Text
2. Ceasar Decode Text
3. Encrypt PDF
4. Decrypt PDF
5. Encrypt Folder (EncFS)
6. Mount Encrypted Folder
7. Exit
</code></pre>

<h2> Ceasar Cipher Usage</h2>

<ul>
  <li>Encodes any text file with a shift you provide</li>
  <li>Stores <code>Shift:N</code> at the top of the file for auto-decoding</li>
</ul>

<h3>Example</h3>

- Input: <code>document.txt</code>  
- Output: <code>document_enc.txt</code>

Then decode → output: <code>document_dec.txt</code>

<h2>PDF Protection</h2>

<ul>
  <li>Encrypts PDFs with a password using <code>PyPDF2</code></li>
  <li>Decrypts PDFs with the correct password</li>
</ul>

<h3>Example</h3>

- Input: <code>contract.pdf</code>  
- Output: <code>contract_enc.pdf</code>  
- Then decrypt → <code>contract_dec.pdf</code>

<h2>Folder Encryption (EncFS)</h2>

<ul>
  <li>Encrypts folders without changing contents</li>
  <li>Does NOT zip, rename, or modify files</li>
  <li>Uses <code>encfs</code> for true on-demand file encryption</li>
</ul>

<h3>Encrypt</h3>

- Input: <code>project/</code>  
- Output: <code>project_encrypted/</code>

<h3>Decrypt</h3>

- Input: <code>project_encrypted/</code>  
- Output: <code>project_decrypted/</code> (automatically extracted)

<h2>🛠 Requirements</h2>

<h3>Python Modules</h3>

<pre><code>pip install PyPDF2 colorama</code></pre>

<h3>System Tools</h3>

<pre><code>sudo apt update
sudo apt install encfs</code></pre>

<h2>Installation</h2>

1. Simply install using the python pip package but first make sure you use Virtal Environment and source the activate:

```bash
python -v venv venv

# Bash / Zsh
source venv/bin/activate

# Fish shell
source venv/bin/activate.fish

# C shell (csh / tcsh)
source venv/bin/activate.csh

```
#### Install Ceasar-toolkit
```bash
pip install ceasar-toolkit
```
Then simply call ``ceasar``in your commands.

2. Clone the project and run:

<pre><code>git clone https://github.com/yourname/Ceasar-cipher-toolkit.git
cd Ceasar-cipher-toolkit
python main.py
</code></pre>

<h2>License</h2>

Released under the <a href="LICENSE">MIT License</a>.

</body>
</html>
