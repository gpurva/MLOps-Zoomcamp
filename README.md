# MLOps-Zoomcamp

Started learning MLOps and Upskilling myself

##Day 1: Environment Configuration

a. Learned Configuring Environment with GitHub Codespaces (VS Code)

b. Add, commit and push our updated work to git repository (use of git status and git diff)

c. Created homework 1 jupyter notebook - Loaded the taxi data, imported sklearn and pandas library

##Day 2: Environment Preparation

a. Created an EC2 Instance: 
Launches a virtual machine in AWS with your chosen OS (Ubuntu, etc.). Acts as your remote server—the place where your model will eventually run in production. You control the hardware (CPU/GPU), OS, storage, and networking. This server can host your ML model as a REST API or batch inference pipeline. You can deploy using Docker, serve with FastAPI, and manage traffic with a load balancer.

b. Used Git Bash to Connect to Instance (SSH): 
Establishes a secure connection to your EC2 instance using your .pem private key. You need command-line access to install software, run code, configure the server. SSH is how you'll manage, debug, and update production services. It’s also how you can automate deployments via CI/CD pipelines.

c. Cloned a GitHub Repo: 
Downloads the codebase (e.g., ML model training scripts, inference logic) from GitHub into the EC2 instance. Brings your project code (or any public codebase like mlops-zoomcamp) to the server where it will be run. This is the source code for your model training or serving pipeline. You’ll often automate this in production using GitHub Actions or Git pull in CI/CD.

d. Connected VS Code to EC2 via Remote SSH: 
Lets you open and edit files on the EC2 server directly in your local VS Code editor. Provides a powerful, user-friendly interface to develop, test, and debug code on the remote instance. You don’t need to constantly SSH and use Vim/Nano—faster development! Essential for building, maintaining, and troubleshooting production code. DevOps/ML engineers often rely on this setup for remote development.

e. Created a Jupyter Notebook in EC2 & Port Forwarded to Local Machine using VS: Runs a Jupyter Notebook server inside the EC2. Port forwarding via VS Code tunnels EC2’s port (e.g., 8888) to your local browser so you can access the notebook like it’s running locally. Jupyter notebooks are great for interactive model development and experimentation. Running them in EC2 gives you access to server-level compute (e.g., GPU instances) while developing in a familiar UI. Notebooks are used to: Test code before converting it into production pipelines, Visualize model outputs and performance, Prepare training data and validate preprocessing. You don't use notebooks in production directly, but they’re crucial for R&D and reproducibility.


