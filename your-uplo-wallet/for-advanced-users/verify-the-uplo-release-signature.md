# Verify the Uplo release signature

All Uplo release binaries are signed, which allows you to confirm that the version you've downloaded is indeed the exact version that we've released. This is an extra security check to ensure you're using legit, unmodified software, which can be pretty important when the app also handles money like UploCoins.

{% hint style="info" %}
These instructions are valid for Uplo v1.0.1 We'll update this as new versions come out, but you can always find the most up-to-date instructions on the Uplo [Get Started](https://uplo.tech/get-started) page, just under the download links.
{% endhint %}

You can download the signing key [here](https://uplo.tech/releases/uplo-signing-key.asc), and the signed hashes for the current release [here](https://uplo.tech/releases/Uplo-v1.5.0-SHA256SUMS.txt.asc).

1. Download and import the Uplo signing key. `wget -c https://uplo.tech/releases/uplo-signing-key.asc` `gpg --import uplo-signing-key.asc`
2. Download the signed hash file, and verify the signature. `wget -c https://uplo.tech/releases/Uplo-v1.5.0-SHA256SUMS.txt.asc` `gpg --verify Uplo-v1.5.0-SHA256SUMS.txt.asc`
3. If you downloaded a zip file, unzip that first. `unzip Uplo-v1.5.0-linux-amd64.zip`
4. Check that the files you downloaded were signed. `sha256sum --check --ignore-missing Uplo-v1.5.0-SHA256SUMS.txt.asc`

You should see "OK" next to the files you did download and errors for the files you have not downloaded.

