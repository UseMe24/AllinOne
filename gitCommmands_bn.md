# Git Commands Full Guide (বাংলা Definitions)

## 1️⃣ git init
**Command এর মানে:** নতুন Git repository তৈরি করা  
**ব্যবহার:** বর্তমান ফোল্ডারকে Git দ্বারা ট্র্যাক করার যোগ্য বানানো  
**কেন:** প্রোজেক্টের পরিবর্তনগুলি version control করতে  
**কখন:** নতুন প্রোজেক্ট শুরু করার সময়  
`git init`

---

## 2️⃣ git clone <repo_url>
**Command এর মানে:** বিদ্যমান remote repository copy করা  
**ব্যবহার:** GitHub বা অন্য সার্ভার থেকে প্রোজেক্ট ডাউনলোড করা  
**কেন:** অন্যদের প্রোজেক্টে কাজ শুরু করতে  
**কখন:** প্রোজেক্ট কাজের শুরুতে  
`git clone git@github.com:UseMe24/MyRepo.git`

---

## 3️⃣ git status
**Command এর মানে:** Local repository-র status দেখা  
**ব্যবহার:** কোন ফাইল modify, staged বা untracked আছে তা জানার জন্য  
**কেন:** কোন ফাইল commit বা push করতে হবে তা জানতে  
**কখন:** কাজের মাঝখানে বা push করার আগে  
`git status`

---

## 4️⃣ git add <file> / git add .
**Command এর মানে:** ফাইল commit-এর জন্য stage করা  
**ব্যবহার:** Git শুধুমাত্র stage করা ফাইল commit করে  
**কেন:** commit-এর জন্য changes select করতে  
**কখন:** commit করার আগে  
`git add newfile.py`  
`git add .`

---

## 5️⃣ git commit -m "message"
**Command এর মানে:** Stage করা changes commit করা  
**ব্যবহার:** পরিবর্তনের snapshot save করা  
**কেন:** Local history track করতে  
**কখন:** add করার পরে, push করার আগে  
`git commit -m "Add login feature"`

---

## 6️⃣ git log / git log --oneline
**Command এর মানে:** Commit history দেখা  
**ব্যবহার:** কোন পরিবর্তন কখন, কে করেছে তা দেখতে  
**কেন:** Debug বা history review করতে  
**কখন:** দরকার হলে  
`git log`  
`git log --oneline`

---

## 7️⃣ git branch / git branch <name>
**Command এর মানে:** Branch দেখা / তৈরি করা  
**ব্যবহার:** আলাদা feature/fix branch তৈরি করা  
**কেন:** main branch safe রাখা  
**কখন:** নতুন feature বা bugfix শুরু করার সময়  
`git branch`  
`git branch feature-login`

---

## 8️⃣ git checkout <branch> / git checkout -b <branch>
**Command এর মানে:** Branch switch করা / create+switch  
**ব্যবহার:** আলাদা branch-এ কাজ করা  
**কেন:** main branch-এর code safe রাখা  
**কখন:** নতুন feature branch এ যাওয়ার সময়  
`git checkout main`  
`git checkout -b feature-login`

---

## 9️⃣ git merge <branch>
**Command এর মানে:** Branch merge করা  
**ব্যবহার:** Feature/fix main branch-এ যোগ করা  
**কেন:** Final version তৈরি করতে  
**কখন:** Feature/fix complete হলে  
`git checkout main`  
`git merge feature-login`

---

## 🔟 git remote -v
**Command এর মানে:** Remote repository URL দেখা  
**ব্যবহার:** Push/Pull target verify করা  
**কেন:** সঠিক remote-এ connect আছে কি না চেক করতে  
**কখন:** প্রোজেক্ট setup বা troubleshooting সময়  
`git remote -v`

---

## 1️⃣1️⃣ git remote add origin <repo_url>
**Command এর মানে:** Remote repository add করা  
**ব্যবহার:** Local repo GitHub/remote-এর সাথে connect করা  
**কেন:** Push/Pull করতে  
**কখন:** নতুন repo connect করার সময়  
`git remote add origin git@github.com:UseMe24/MyRepo.git`

---

## 1️⃣2️⃣ git push / git push -u origin main
**Command এর মানে:** Local commits remote-এ পাঠানো  
**ব্যবহার:** Local changes GitHub-এ sync করা  
**কেন:** সবাইকে update রাখতে  
**কখন:** Commit করার পরে  
`git push`  
`git push -u origin main`

---

## 1️⃣3️⃣ git pull / git pull --rebase
**Command এর মানে:** Remote changes download + merge  
**ব্যবহার:** Local copy update রাখা  
**কেন:** Online changes নিয়ে sync করতে  
**কখন:** কাজ শুরু করার আগে বা push করার আগে  
`git pull`  
`git pull --rebase`

---

## 1️⃣4️⃣ git fetch
**Command এর মানে:** Remote changes download কিন্তু merge না করা  
**ব্যবহার:** Update check করা  
**কেন:** Local file safe রাখতে  
**কখন:** Remote changes detect করতে  
`git fetch origin`

---

## 1️⃣5️⃣ git diff / git diff origin/main
**Command এর মানে:** File বা commit এর পরিবর্তন দেখা  
**ব্যবহার:** Changes review করা  
**কেন:** Commit করার আগে changes verify করতে  
**কখন:** Add/commit আগে  
`git diff`  
`git diff origin/main`

---

## 1️⃣6️⃣ git reset HEAD <file> / git reset --hard
**Command এর মানে:** Stage থেকে remove / discard changes  
**ব্যবহার:** ভুল commit বা stage ঠিক করা  
**কেন:** Safety এবং clean history রাখতে  
**কখন:** ভুল stage/commit করলে  
`git reset HEAD <file>`  
`git reset --hard`

---

## 1️⃣7️⃣ git rm <file>
**Command এর মানে:** Tracked file remove করা  
**ব্যবহার:** Obsolete file delete করা  
**কেন:** Repo clean রাখতে  
**কখন:** ফাইল obsolete হলে  
`git rm oldfile.py`  
`git commit -m "Remove oldfile"`

---

## 1️⃣8️⃣ git stash / git stash apply
**Command এর মানে:** Temporary changes save / restore করা  
**ব্যবহার:** Branch switch করতে কাজ incomplete থাকলে  
**কেন:** Interrupt হলে কাজ lose না করতে  
**কখন:** জরুরি branch switch করতে হলে  
`git stash`  
`git stash apply`

---

## 1️⃣9️⃣ git tag <tag_name>
**Command এর মানে:** Commit mark / version  
**ব্যবহার:** Release version mark করা  
**কেন:** Project release management  
**কখন:** v1.0, v2.0 release  
`git tag v1.0`  
`git push origin v1.0`

---

## 2️⃣0️⃣ git log --graph --oneline --all
**Command এর মানে:** Commit & branch structure visualize  
**ব্যবহার:** Branching ও history বোঝার জন্য  
**কেন:** Conflicts, merge & workflow সহজে দেখার জন্য  
**কখন:** Debug বা review করতে  
`git log --graph --oneline --all`

---

## 2️⃣1️⃣ git config --global
**Command এর মানে:** User, email, editor configure করা  
**ব্যবহার:** Git identity set করা & editor select করা  
**কেন:** Proper commit & editor selection  
**কখন:** প্রথম setup বা preference change  
`git config --global user.name "UseMe24"`  
`git config --global user.email "youremail@example.com"`  
`git config --global core.editor vim`

---

💡 **Offline Usage Tips:**  
- Offline-এ সব command কাজ করবে except push/pull/fetch  
- Later online push/pull করতে হবে  
- SSH use করলে password/token hassle নেই
