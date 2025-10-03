Here's your content formatted as a clean, professional document titled **"🐧 Basic Linux Commands on Azure VM"** — suitable for sharing, saving as a `.md`, `.pdf`, or `.docx` file:

---

# 🐧 Basic Linux Commands on Azure VM

## 1. Azure VM Setup

* **Operating System:** Ubuntu Server 24.04 LTS
* **NSG (Network Security Group) Rules:**

  * `22/tcp` → SSH
  * `80/tcp` → HTTP
  * `443/tcp` → HTTPS

---

## 2. SSH Connection

### Step 1: Set Permissions for Your SSH Key

```bash
cd Downloads
chmod 400 key.pem
```

### Step 2: Connect to the Azure VM

```bash
ssh -i "key.pem" atul@<PUBLIC_IP>
```

**Example:**

```bash
ssh -i key.pem atul@172.179.236.162
```

---

## 3. Basic Linux Commands Practice

```bash
clear               # Clear screen
ls                  # List files and directories
mkdir project       # Create directory
ls
touch a.txt         # Create a new file
ls
mv a.txt project/   # Move file to project directory
ls
pwd                 # Print current working directory
cd project/         # Change to project directory
pwd
ls
sudo nano a.txt     # Edit file using nano
cat a.txt           # View content of a.txt
touch b.txt         # Create another file
cat b.txt           # View content of b.txt (will be empty)
ls
cp a.txt b.txt      # Copy a.txt to b.txt
ls
cat b.txt           # Verify content of b.txt
ls
rm b.txt            # Delete b.txt
ls
cd ..               # Go back to previous directory
ls
rm -rf project/     # Delete project directory recursively
ls
history             # Show command history
```

---

## 4. Install Packages

```bash
sudo apt install snap -y
sudo snap install tree
sudo snap install docker
sudo apt install git -y
```

---

## 5. Verify Versions

```bash
docker --version
git --version
```

---

## 6. Git Workflow Example

```bash
git init                   # Initialize a new git repository
touch a.txt                # Create a file
git add a.txt              # Stage the file
git commit -m "added code" # Commit the file
git branch -M main         # Rename default branch to main
```

### Clone and Update Repository

```bash
git clone https://github.com/atulkamble/AzureVM-Linux.git
cd AzureVM-Linux
git pull
```

### Run and Update Python File

```bash
python3 helloworld.py      # Run Python script
nano helloworld.py         # Edit Python script
python3 helloworld.py      # Run updated script
git add .                  # Stage all changes
git commit -m "updated code"
git push origin main       # Push to GitHub
```

---

Let me know if you’d like this exported to **PDF**, **Markdown**, or **Word** format!
# test1
