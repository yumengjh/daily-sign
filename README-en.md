# 🕒 Daily Check-in

Automatically commit to your repository every day.

## Step 1: Fork this repository

Click the **“Fork”** button in the top-right corner to copy this repo to your own GitHub account.

------

## Step 2: Add Secrets

Go to your repository →
 **Settings → Secrets and variables → Actions → New repository secret**

Add the following two secrets:

| Name         | Example Value | Description                                             |
| ------------ | ------------- | ------------------------------------------------------- |
| `USERNAME`   | `yumengjh`    | Your GitHub username (case-sensitive)                   |
| `PUSH_TOKEN` | `ghp_xxx...`  | Your Personal Access Token (PAT) with `repo` permission |

### How to create a PAT

1. Visit https://github.com/settings/tokens
2. Click **“Generate new token (classic)”**
3. Check the **repo** permission
4. Generate and copy your token (save it securely)

------

## Step 3: Automatic Daily Check-in

This workflow runs **every day at 00:00 (Beijing Time)**
 → *(16:00 UTC)*

It automatically appends the current date and time to your **README.md** file like this:

```
- 2025-10-10 00:00:00
```

------

## Record Section ↓

```
## record
- date
```
