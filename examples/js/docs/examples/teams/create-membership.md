let sdk = new Appwrite();

sdk
    .setProject('5df5acd0d48c2') // Your project ID
;

let promise = sdk.teams.createMembership('[TEAM_ID]', 'email@example.com', [], 'https://example.com');

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});