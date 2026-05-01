# Team Patch Ideas

These are safe, small edits teammates can make later so everyone has visible commit history. They should pick one item each and keep the change focused.

## Mehak

Suggested patch:

- Improve wording on the home page feature cards in `templates/index.html`.
- Add one extra documentation paragraph to `RENDER_DEPLOYMENT.md`.

## Jashanjot Singh

Suggested patch:

- Add one more SQL injection explanation sentence to `templates/security_demo.html`.
- Add a short comment near one parameterized query in `app.py`.

## Jashan Yadav

Suggested patch:

- Adjust the brute-force demo wording in `templates/security_demo.html`.
- Add one extra expected test case to the evaluation study guide.

## Aryan Gupta

Suggested patch:

- Improve the transfer page helper text in `templates/transfer.html`.
- Add one sentence explaining CSRF in `templates/security_demo.html`.

## Vanshika Sardana

Suggested patch:

- Improve the password hashing explanation on the Security Demo Lab.
- Add one future-improvement bullet about removing the legacy `password` column.

## Raghav Verma

Suggested patch:

- Add a small access-control note to the Security Demo Lab.
- Add one route-level comment near the statement access-control check.

## Safe Rules for These Patches

- Do not change database names or route URLs.
- Do not commit real secrets.
- Keep each patch small.
- Run the app after editing and check `http://127.0.0.1:5001/`.
