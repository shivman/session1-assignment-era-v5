# ERA V5 Session 1 Assignment — Interactive Web App

Static browser app with **real gradient-descent training** (no libraries, no hardcoded numbers).

## What it proves

| Section | Claim | What you see |
|---------|-------|--------------|
| **S1-1** | Activations exist for a reason | ~300 concentric-ring points; linear ≈ 50–55% acc, ReLU hidden layer ≈ 99%+ |
| **S1-2** | Depth without nonlinearity is a lie | 1-layer vs 5-layer linear = same straight boundary; 5-layer + ReLU solves rings; matrix product bonus |
| **S1-3** | Embeddings learn similarity from next-token | Toy grammar (cat/dog/cow, apple/mango, eat/chase/see); 2D embedding clusters by category |
| **S1-4** | Data closes the generalization gap | Over-parameterized net; huge train–test gap at n=20, shrinks at n=2000 |

## Run locally

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8080
# visit http://localhost:8080
```

S1-1 through S1-3 auto-train on load. Click **Train all sizes** for S1-4 (~15 seconds).

## Deploy to Netlify (for submission)

1. Go to [https://app.netlify.com](https://app.netlify.com) and sign up / log in.
2. Drag and drop the `era_v5_session1_assignment` folder onto the deploy area.
3. Copy the public URL (e.g. `https://your-site-name.netlify.app`).
4. Test in an **incognito window** to confirm it's public.
5. Submit on Axiom:
   - **URL:** your Netlify link
   - **Caption:** `Interactive web app proving Session 1 concepts: activations, linear depth collapse, emergent embeddings, and data vs memorization`
   - Check the incognito accessibility box

No build step required.
