in vite.config.js file update this section

export default defineConfig({
  plugins: [vue()],
  base: process.env.NODE_ENV === 'production'
    ? '/todo/'
    : '/'
})

$ ls -al ~/.ssh
# Lists the files in your .ssh directory, if they exist

Generating a new SSH key
$ ssh-keygen -t ed25519 -C "libin.babu@altd.in"
> Generating public/private ALGORITHM key pair.
> Enter a file in which to save the key (/c/Users/YOU/.ssh/id_ALGORITHM):[Press enter]
> Enter passphrase (empty for no passphrase): [Type a passphrase]
> Enter same passphrase again: [Type passphrase again]

Adding your SSH key to the ssh-agent
# start the ssh-agent in the background
$ eval "$(ssh-agent -s)"
> Agent pid 59566

$ ssh-add ~/.ssh/id_ed25519

Switching remote URLs from HTTPS to SSH
$ git remote -v
> origin  https://github.com/libinann2020/todo.git (fetch)
> origin  https://github.com/libinann2020/todo.git (push)

$ git remote set-url origin git@github.com:libinann2020/todo.git

$ git remote -v
# Verify new remote URL
> origin  git@github.com: libinann2020/todo.git (fetch)
> origin  git@github.com: libinann2020/todo.git (push)

$ clip < ~/.ssh/id_ed25519.pub
  # Copies the contents of the id_ed25519.pub file to your clipboard

  in github repository
  -In the upper-right corner of any page, click your profile photo, then click Settings.
-In the "Access" section of the sidebar, click  SSH and GPG keys.
-Click New SSH key.
-In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal laptop, you might call this key "Personal laptop".
-Select the type of key, either authentication or signing.
-Paste your public key into the "Key" field.
-Click Add SSH key.

$ npm install -g gh-pages

switch branch to gh-pages
Now go into Settings, scroll down and and ensure gh-pages is listed as the Source.