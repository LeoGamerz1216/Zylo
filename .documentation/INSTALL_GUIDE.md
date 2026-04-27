# 🛠 Zylo Installation & Troubleshooting
> **How to get Zylo running on any machine, even with slow connections.**

Because **Zylo** is a premium, heavy-duty application with a massive set of custom icons and dependencies, standard installation commands might fail. Use this guide to ensure a smooth setup.

---

## 1. Prerequisites
Before you start, ensure your environment is ready:
* **Node.js:** LTS version (v18+ recommended).
* **Yarn:** Global installation (`npm install --global yarn`).
* **Git:** To clone the latest source.

## 2. Standard Setup
```bash
# Clone the repository
git clone [https://github.com/YourUsername/Zylo.git](https://github.com/YourUsername/Zylo.git)
cd Zylo

# Install dependencies
yarn install
3. Troubleshooting "Network Trouble" (The Timeout Fix)
If you see the error ESOCKETTIMEDOUT or a "Retrying..." loop during the @fortawesome icon download, your connection is timing out. Use the Zylo Force Install command:

Bash
yarn install --network-timeout 1000000 --network-concurrency 1
Why this works:

--network-timeout 1000000: Increases the wait time to ~16 minutes.

--network-concurrency 1: Forces Yarn to download one file at a time, preventing your connection from choking.

4. Running the Development Environment
Once the packages are installed, launch the app:

Bash
yarn run dev
5. Building for Production
To create your own .exe (Windows), .dmg (Mac), or .AppImage (Linux):

Bash
yarn run build
The final installer will be located in the dist/ or build/ folder.

Still having issues?
Registry Swap: If Yarn's registry is slow, try: yarn config set registry https://registry.npmjs.org/

Clean Cache: Run yarn cache clean before retrying.

Developed by Pavan Tej | Oasis Centers India