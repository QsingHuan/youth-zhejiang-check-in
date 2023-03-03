# Youth Zhejiang Check-in

## Get started

### Config

1. Copy `config.toml.demo` to `config.toml`
2. Get `openid`, and set the `user/username/openid` field.
3. Normally, `nid` and `cardNo` can be acquired automatically if you have checked in before, so you don't have to fill them in.
   * If there is something wrong, you can fill these fields.
4. To check in for multiple users, add another `[user.yyy]`.

### Run

```bash
pip install -r requirements.txt

python main.py
```
