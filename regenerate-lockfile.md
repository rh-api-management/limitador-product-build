## How to generate RPM Lockfile


1. `subscription-manager register --org="your-org-id" --activationkey="your-activation-key"`
2. `DNF_VAR_SSL_CLIENT_KEY=/etc/pki/entitlement/YOUR_CERT-key.pem DNF_VAR_SSL_CLIENT_CERT=/etc/pki/entitlement/YOUR_CERT.pem rpm-lockfile-prototype rpms.in.yaml  --image=YOUR_BASE_IMAGE`