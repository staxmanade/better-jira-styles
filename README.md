
# For more context/details see [this blog post](http://staxmanade.com/2016/09/better-compact-jira-board-u-i-/)


# How to get setup

1. Install a CSS style plugin into your browser. This post all use [Stylebot](https://chrome.google.com/webstore/detail/stylebot/oiaejidbmkiecgbjeifoejpgmdaleoha?hl=en) for the Chrome web browser.

  - Just install the plugin from the Chrome store by [clicking this link](https://chrome.google.com/webstore/detail/stylebot/oiaejidbmkiecgbjeifoejpgmdaleoha?hl=en) and selecting `[+ ADD TO CHROME]` button on the upper right of the page.

2. Once the plugin is installed. Close all tabs and re-open a tab to the JIRA kanban board.

3. Click the new Stylebot plugin `CSS` button and the `Open Stylebot...` option in your chrome browser toolbar which will open up a U.I. that allow you to mess around with the page's style.

4. At the bottom of the Stylebot click `Edit CSS` which will give you a blank text box you can write custom CSS into.

5. Paste in the following CSS and hit `Save`

```css

/** Version 2.0
 ** Copyright Jason Jarrett
 **/

.ghx-avatar-img {
    font-size: 15px;
    height: 15px;
    line-height: 15px;
    width: 15px;
}

.ghx-band-1 .ghx-issue .ghx-avatar {
    left: 100px;
    right: auto;
    top: -3px;
}

.ghx-band-3 .ghx-issue .ghx-avatar {
    top: 0px;
}

.ghx-issue .ghx-extra-fields {
    margin-top: 5px;
}

.ghx-issue .ghx-flags {
    left: 20px;
    top: 5px;
}

.ghx-issue .ghx-highlighted-fields {
    margin-top: 5px;
}

.ghx-issue .ghx-type {
    left: 5px;
    top: 5px;
}

.ghx-issue-content {
    font-size: 12px;
    margin-top: 3px;
    padding: 5px;
}

.ghx-issue-fields .ghx-key {
    margin-left: 30px;
}

.ghx-issue.ghx-has-avatar .ghx-issue-fields, .ghx-issue.ghx-has-corner .ghx-issue-fields {
    padding-right: 0px;
}

/* the below adjusts the backlog view */

.ghx-backlog-column .ghx-plan-extra-fields.ghx-row {
    float: right;
    position: relative;
    right: 70px;
    margin: 0;
    margin-top: -15px;
    height: 18px;
}

.ghx-backlog-column .ghx-issue-content, .ghx-backlog-column .ghx-end.ghx-row {
    padding: 0;
    margin: 0;
}

/* filters */
.js-quickfilter-button {
    padding: 0;
}
.js-sprintfilter {
    white-space: nowrap;
}
.js-sprintfilter > span {
    padding: 0;
}
dl dt, dd {
    margin: 0;
    padding: 0;
}

```
