## How to test custom filter update

1. Install
run command in terminal `git clone git@github.com:maximtop/ag-test-custom-filter-update.git`
go to created folder `cd ag-test-custom-filter-update`
inside your folder run `yarn install`

2. Start local server
`yarn start`

3. Add custom filter to the extension
link to the filter - `http://localhost:5000/rules.txt`

4. Test custom filter update
Open in your editor `rules.txt`

Change text of rules.txt and update filters in the extension
filters should update only when text of rules has changed or if filter has version tag
version updated

## Version tag
Version tags looks like

`! Version: 2.10.0.2`

add this line after filter title, if you'll increase version number and update filters in the extension, filter should update, otherway, not
