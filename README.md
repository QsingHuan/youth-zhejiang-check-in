# Youth Zhejiang Check-in

## Get started

### Config

1. Copy `config.toml.demo` to `config.toml`
2. Get the open-id, and set the `user/username/openid` field.
3. Normally, `nid` and `cardNo` can be acquired automatically if you have checked in before, so you don't have to fill them in.
   * If there is something wrong, you can fill in these fields.
4. For multiple users, add another `[user.yyy]`.

### Run

```bash
pip install -r requirements.txt

python main.py
```

### Actions

This tool supports GitHub Actions.

1. Fork this repo.
2. Set secrets `OPENID` as your open-id.
    * If you have multiple users, separate the open-ids with `,`, for example, `oO-user1xxxx,oO-user2yyyy,oO-user3zzzz`.
    * Custom nid and cardNo are currently unsupported for Actions mode.
3. The workflow will be run at 23:11 every Monday and Friday.
