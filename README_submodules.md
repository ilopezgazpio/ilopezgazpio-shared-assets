# Shared assets for drone websites

## Manual Update in Each Secondary Repo

1. Navigate to secondary repo
2. git submodule update --remote --merge

## Initialize submodule

git submodule add https://github.com/your-username/shared-assets.git assets

## If cloning for the first time, run

git clone --recurse-submodules https://github.com/your-username/secondary-repo.git

## To initialize a submodule, run

git submodule init
git submodule update