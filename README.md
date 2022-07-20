# Getting Started

-Git clone this project
- npm install
- npm run storybook




storybook is only used for building UI components and keeping them isolated from the react application(business logic). These components can be easily visualized when you run the storybook through this npm run storybook (windows) or yarn storybook(mac/ubuntu) command. It runs on a different port unlike npm start runs on the 3000 port by default.

These components are then imported into the main react application. React will use these components based on the requirement. Storybook gives you the ability to browse all the UI components that you have built and then later react will use it. This allows you to develop one component at a time.

What will happen when you execute the command npm run storybook?

This command at first will search for main.js and if found it will look for all the file which extends with stories.js which is nothing but the stories that you have built. It will then create a list of stories in any order or specified order which will be shown in the storybook webpage at 6006 port by default.

Why we don't use npm start for running the storybook?

We can use npm start for running the storybook but you need to configure it in the package.json file under the "scripts" as shown below.

"scripts": {
    "start": "start-storybook -p 6006 -s public"
  }
Here public means that this storybook doesn't require any authentication for running it. Now if you do npm start it will only run the storybook for you, not the react application. This storybook can be used later in different react applications.

I'll recommend that if you are implementing some basic concept of storybook then it is better to run both separately on a different port.

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
