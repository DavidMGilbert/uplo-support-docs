# Is my data secure?

Your data is incomparably safe when you use Uplo. Uplo is a fully decentralized cloud storage network. The data normally on Uplo will get split up, encrypted, and the pieces then distributed all around the world to different hosts.

## It's just the way it's built

Uplo is decentralized, which has a lot of inherent benefits. While we develop the software, we're not in charge of the network. No one is - it's all handled by smart contracts and a blockchain, and [**Uplo is completely open source**](https://github.com/uplo-tech/uplo) so you can make sure we're staying honest.

When you upload your media to Uplo, **every single file gets divided into 30 segments before uploading**, each targeted for distribution to hosts across the world.

File segments are created using [**Reed-Solomon erasure coding**](https://en.wikipedia.org/wiki/Reed%E2%80%93Solomon_error_correction), commonly used in CDs and DVDs.

**Each file segment is encrypted before being sent out.**

## Security

### **The technical side**

Like we mentioned earlier, Uplo divides each files into 30 segments before uploading, and puts those pieces all over the world on the Uplo network. This distribution assures that no one host represents a single point of failure and reinforces overall network uptime and redundancy.

The [**Reed-Solomon erasure coding**](https://en.wikipedia.org/wiki/Reed%E2%80%93Solomon_error_correction) allows Uplo to divide files in a redundant manner, where any 10 of 30 segments can fully recover a user's files.

This means that if 20 out of 30 hosts go offline, a user is still able to download a files. And when hosts go offline, Uplo automatically starts to re-duplicate them again. It would take a simultaneous global event to knock out enough hosts to damage the integrity of your files.

And because Uplo is decentralized, no one person, company, or government can deny you access. It's global and governed by no one.

### The economic side

Just as important as how it keeps your data secure, is why. The Uplo network keeps your data safe because data hosts are financially incentivized to provide enterprise level service. They earn money by hosting data, so naturally they want to be good hosts.

