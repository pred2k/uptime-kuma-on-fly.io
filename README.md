# run uptime-kuma on fly.io

- https://github.com/louislam/uptime-kuma
- on
- https://fly.io/

# prepare

1. create account @ https://fly.io/app/sign-up

1. add credit-card to account (yes, even if its on free tier)

1. install flyctl
   `brew install flyctl`

1. connect flyctl with account
   `fly auth login`

## deploy

    flyctl launch

## serv unter status subdomain

    flyctl certs create status.mydomain.com

## update update-kuma

1. update image version in `fly.toml`
2. run: `flyctl deploy`
