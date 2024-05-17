# rust-nix-template
A simple template on How to use nix to develop rust projects. I may add other languages in the future

## Usage
1. You need to add the flake.nix, toolchain.toml and .envrc into your project
2. You need to change self'.devShells.hello-world to self'.devShells.your-project-name
4. You need to enter ``nix develop`` in the terminal and after building run ``cargo generate-lockfile``
5. Now you can use ``nix build`` and ``nix run``

## Important Notice 
1. Dont forget to always commit before executing commands as nix doesnt recognise uncommited files
2. It is not truly deterministic as the source code and dependencies can change
3. dont forget to update the lockfile from time to time so it doesnt grow old (You dont have to tho)
