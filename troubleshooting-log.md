# Troubleshooting Log - Lab 1.5

---

## Issue 1: Missing User Home Directories
- **Symptom:** After creating users, `ls -la /home/` did not list `alice`, `bob`, or `charlie`.
- **Diagnosis:** Checked `/etc/passwd` entries → users existed but home directories were not properly created.
- **Resolution:**  
  ```bash
  sudo mkdir -p /home/alice /home/bob /home/charlie
  sudo chown alice:alice /home/alice
  sudo chown bob:bob /home/bob
  sudo chown charlie:charlie /home/charlie
