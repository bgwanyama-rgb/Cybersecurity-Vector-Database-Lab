# Step 4 — Create an OpenAI API Key

Some AI integrations in this project may require an OpenAI API key.

---

## 1. Create an OpenAI Account

Go to:

https://platform.openai.com/

Sign up or log in.

---

## 2. Generate an API Key

Navigate to:

https://platform.openai.com/api-keys

Click:

```
Create new secret key
```

Copy the key.

Example format:

```
sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

---

## 3. Add the API Key to your Environment

We store the key as an environment variable.

### Windows (PowerShell)

```powershell
setx OPENAI_API_KEY "your_api_key_here"
```

Restart VS Code after running this.

---

### Mac / Linux

Add to your shell profile:

```bash
export OPENAI_API_KEY="your_api_key_here"
```

Then reload:

```bash
source ~/.bashrc
```

or

```bash
source ~/.zshrc
```

---

## 4. Verify the Key Works

Run in Python:

```python
import os

print(os.getenv("OPENAI_API_KEY"))
```

If the key prints, setup is successful.

---

## Security Note

Never commit your API key to GitHub.

The key should always remain in:

- environment variables
- `.env` files (ignored by Git)

---

## Optional: Using a `.env` file

Create:

```
.env
```

Add:

```
OPENAI_API_KEY=your_api_key_here
```

Install dotenv:

```bash
pip install python-dotenv
```

Load in Python:

```python
from dotenv import load_dotenv
load_dotenv()
```
