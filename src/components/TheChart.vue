
<script>
import { HorizontalBar } from "vue-chartjs";
import CHARTSJS from "vue-chartjs";

export default {
  extends: HorizontalBar,
  data() {
    return {
      chartData: {
        labels: [
          "2015-01",
          "2015-02",
          "2015-03",
          "2015-04",
          "2015-05",
          "2015-06",
          "2015-07",
          "2015-08",
          "2015-09",
          "2015-10",
          "2015-11",
          "2015-12",
        ],
        datasets: [
          {
            label: "Bar Chart",
            borderWidth: 1,
            backgroundColor: [
              "rgba(255, 99, 132, 0.2)",
              "rgba(54, 162, 235, 0.2)",
              "rgba(255, 206, 86, 0.2)",
              "rgba(75, 192, 192, 0.2)",
              "rgba(153, 102, 255, 0.2)",
              "rgba(255, 159, 64, 0.2)",
              "rgba(255, 99, 132, 0.2)",
              "rgba(54, 162, 235, 0.2)",
              "rgba(255, 206, 86, 0.2)",
              "rgba(75, 192, 192, 0.2)",
              "rgba(153, 102, 255, 0.2)",
              "rgba(255, 159, 64, 0.2)",
            ],
            borderColor: [
              "rgba(255,99,132,1)",
              "rgba(54, 162, 235, 1)",
              "rgba(255, 206, 86, 1)",
              "rgba(75, 192, 192, 1)",
              "rgba(153, 102, 255, 1)",
              "rgba(255, 159, 64, 1)",
              "rgba(255,99,132,1)",
              "rgba(54, 162, 235, 1)",
              "rgba(255, 206, 86, 1)",
              "rgba(75, 192, 192, 1)",
              "rgba(153, 102, 255, 1)",
              "rgba(255, 159, 64, 1)",
            ],
            pointBorderColor: "#2554FF",
            data: [12, 19, 3, 5, 2, 3, 20, 3, 5, 6, 2, 1],
          },
        ],
      },
      options: {
        scales: {
          yAxes: [
            {
              ticks: {
                beginAtZero: true,
              },
              gridLines: {
                display: true,
              },
            },
          ],
          xAxes: [
            {
              gridLines: {
                display: false,
              },
            },
          ],
        },
        legend: {
          display: true,
        },
        responsive: true,
        maintainAspectRatio: false,
      },
    };
  },
  mounted() {
    this.renderChart(this.chartData, this.options);
    console.log(CHARTSJS);
  },
};
</script>
/*
// import { Line } from "vue-chartjs";

// export default {
//   extends: Line,
//   mounted() {
//     this.renderChart(
//       {
//         labels: [
//           "January",
//           "February",
//           "March",
//           "April",
//           "May",
//           "June",
//           "July",
//         ],
//         datasets: [
//           {
//             label: "Data One",
//             backgroundColor: "#f87979",
//             data: [40, 39, 10, 40, 39, 80, 40],
//           },
//         ],
//       },
//       { responsive: true, maintainAspectRatio: false }
//     );
//   },
// };

import { Line } from "vue-chartjs";
export default {
  extends: Line,

  data() {
    return {
      options: {
        responsive: true,
        maintainAspectRatio: false,
      },
      chartdata: {
        labels: ["January", "February"],
        datasets: [
          {
            label: "Data One",
            backgroundColor: "#f87979",
            data: [40, 20],
          },
        ],
      },
      records: [
        {
          id: 28457823,
          node_id: "MDEwOlJlcG9zaXRvcnkyODQ1NzgyMw==",
          name: "freeCodeCamp",
          full_name: "freeCodeCamp/freeCodeCamp",
          private: false,
          owner: {
            login: "freeCodeCamp",
            id: 9892522,
            node_id: "MDEyOk9yZ2FuaXphdGlvbjk4OTI1MjI=",
            avatar_url: "https://avatars.githubusercontent.com/u/9892522?v=4",
            gravatar_id: "",
            url: "https://api.github.com/users/freeCodeCamp",
            html_url: "https://github.com/freeCodeCamp",
            followers_url:
              "https://api.github.com/users/freeCodeCamp/followers",
            following_url:
              "https://api.github.com/users/freeCodeCamp/following{/other_user}",
            gists_url:
              "https://api.github.com/users/freeCodeCamp/gists{/gist_id}",
            starred_url:
              "https://api.github.com/users/freeCodeCamp/starred{/owner}{/repo}",
            subscriptions_url:
              "https://api.github.com/users/freeCodeCamp/subscriptions",
            organizations_url: "https://api.github.com/users/freeCodeCamp/orgs",
            repos_url: "https://api.github.com/users/freeCodeCamp/repos",
            events_url:
              "https://api.github.com/users/freeCodeCamp/events{/privacy}",
            received_events_url:
              "https://api.github.com/users/freeCodeCamp/received_events",
            type: "Organization",
            site_admin: false,
          },
          html_url: "https://github.com/freeCodeCamp/freeCodeCamp",
          description:
            "freeCodeCamp.org's open-source codebase and curriculum. Learn to code for free.",
          fork: false,
          url: "https://api.github.com/repos/freeCodeCamp/freeCodeCamp",
          forks_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/forks",
          keys_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/keys{/key_id}",
          collaborators_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/collaborators{/collaborator}",
          teams_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/teams",
          hooks_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/hooks",
          issue_events_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/issues/events{/number}",
          events_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/events",
          assignees_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/assignees{/user}",
          branches_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/branches{/branch}",
          tags_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/tags",
          blobs_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/git/blobs{/sha}",
          git_tags_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/git/tags{/sha}",
          git_refs_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/git/refs{/sha}",
          trees_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/git/trees{/sha}",
          statuses_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/statuses/{sha}",
          languages_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/languages",
          stargazers_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/stargazers",
          contributors_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/contributors",
          subscribers_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/subscribers",
          subscription_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/subscription",
          commits_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/commits{/sha}",
          git_commits_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/git/commits{/sha}",
          comments_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/comments{/number}",
          issue_comment_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/issues/comments{/number}",
          contents_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/contents/{+path}",
          compare_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/compare/{base}...{head}",
          merges_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/merges",
          archive_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/{archive_format}{/ref}",
          downloads_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/downloads",
          issues_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/issues{/number}",
          pulls_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/pulls{/number}",
          milestones_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/milestones{/number}",
          notifications_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/notifications{?since,all,participating}",
          labels_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/labels{/name}",
          releases_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/releases{/id}",
          deployments_url:
            "https://api.github.com/repos/freeCodeCamp/freeCodeCamp/deployments",
          created_at: "2014-12-24T17:49:19Z",
          updated_at: "2021-10-24T04:31:01Z",
          pushed_at: "2021-10-23T22:04:17Z",
          git_url: "git://github.com/freeCodeCamp/freeCodeCamp.git",
          ssh_url: "git@github.com:freeCodeCamp/freeCodeCamp.git",
          clone_url: "https://github.com/freeCodeCamp/freeCodeCamp.git",
          svn_url: "https://github.com/freeCodeCamp/freeCodeCamp",
          homepage: "https://contribute.freecodecamp.org",
          size: 238764,
          stargazers_count: 334170,
          watchers_count: 334170,
          language: "JavaScript",
          has_issues: true,
          has_projects: false,
          has_downloads: true,
          has_wiki: false,
          has_pages: true,
          forks_count: 27138,
          mirror_url: null,
          archived: false,
          disabled: false,
          open_issues_count: 155,
          license: {
            key: "bsd-3-clause",
            name: 'BSD 3-Clause "New" or "Revised" License',
            spdx_id: "BSD-3-Clause",
            url: "https://api.github.com/licenses/bsd-3-clause",
            node_id: "MDc6TGljZW5zZTU=",
          },
          allow_forking: true,
          is_template: false,
          topics: [
            "careers",
            "certification",
            "community",
            "curriculum",
            "d3",
            "education",
            "freecodecamp",
            "hacktoberfest",
            "javascript",
            "learn-to-code",
            "math",
            "nodejs",
            "nonprofits",
            "programming",
            "react",
            "teachers",
          ],
          visibility: "public",
          forks: 27138,
          open_issues: 155,
          watchers: 334170,
          default_branch: "main",
          score: 1,
        },
        {
          id: 11730342,
          node_id: "MDEwOlJlcG9zaXRvcnkxMTczMDM0Mg==",
          name: "vue",
          full_name: "vuejs/vue",
          private: false,
          owner: {
            login: "vuejs",
            id: 6128107,
            node_id: "MDEyOk9yZ2FuaXphdGlvbjYxMjgxMDc=",
            avatar_url: "https://avatars.githubusercontent.com/u/6128107?v=4",
            gravatar_id: "",
            url: "https://api.github.com/users/vuejs",
            html_url: "https://github.com/vuejs",
            followers_url: "https://api.github.com/users/vuejs/followers",
            following_url:
              "https://api.github.com/users/vuejs/following{/other_user}",
            gists_url: "https://api.github.com/users/vuejs/gists{/gist_id}",
            starred_url:
              "https://api.github.com/users/vuejs/starred{/owner}{/repo}",
            subscriptions_url:
              "https://api.github.com/users/vuejs/subscriptions",
            organizations_url: "https://api.github.com/users/vuejs/orgs",
            repos_url: "https://api.github.com/users/vuejs/repos",
            events_url: "https://api.github.com/users/vuejs/events{/privacy}",
            received_events_url:
              "https://api.github.com/users/vuejs/received_events",
            type: "Organization",
            site_admin: false,
          },
          html_url: "https://github.com/vuejs/vue",
          description:
            "🖖 Vue.js is a progressive, incrementally-adoptable JavaScript framework for building UI on the web.",
          fork: false,
          url: "https://api.github.com/repos/vuejs/vue",
          forks_url: "https://api.github.com/repos/vuejs/vue/forks",
          keys_url: "https://api.github.com/repos/vuejs/vue/keys{/key_id}",
          collaborators_url:
            "https://api.github.com/repos/vuejs/vue/collaborators{/collaborator}",
          teams_url: "https://api.github.com/repos/vuejs/vue/teams",
          hooks_url: "https://api.github.com/repos/vuejs/vue/hooks",
          issue_events_url:
            "https://api.github.com/repos/vuejs/vue/issues/events{/number}",
          events_url: "https://api.github.com/repos/vuejs/vue/events",
          assignees_url:
            "https://api.github.com/repos/vuejs/vue/assignees{/user}",
          branches_url:
            "https://api.github.com/repos/vuejs/vue/branches{/branch}",
          tags_url: "https://api.github.com/repos/vuejs/vue/tags",
          blobs_url: "https://api.github.com/repos/vuejs/vue/git/blobs{/sha}",
          git_tags_url: "https://api.github.com/repos/vuejs/vue/git/tags{/sha}",
          git_refs_url: "https://api.github.com/repos/vuejs/vue/git/refs{/sha}",
          trees_url: "https://api.github.com/repos/vuejs/vue/git/trees{/sha}",
          statuses_url: "https://api.github.com/repos/vuejs/vue/statuses/{sha}",
          languages_url: "https://api.github.com/repos/vuejs/vue/languages",
          stargazers_url: "https://api.github.com/repos/vuejs/vue/stargazers",
          contributors_url:
            "https://api.github.com/repos/vuejs/vue/contributors",
          subscribers_url: "https://api.github.com/repos/vuejs/vue/subscribers",
          subscription_url:
            "https://api.github.com/repos/vuejs/vue/subscription",
          commits_url: "https://api.github.com/repos/vuejs/vue/commits{/sha}",
          git_commits_url:
            "https://api.github.com/repos/vuejs/vue/git/commits{/sha}",
          comments_url:
            "https://api.github.com/repos/vuejs/vue/comments{/number}",
          issue_comment_url:
            "https://api.github.com/repos/vuejs/vue/issues/comments{/number}",
          contents_url:
            "https://api.github.com/repos/vuejs/vue/contents/{+path}",
          compare_url:
            "https://api.github.com/repos/vuejs/vue/compare/{base}...{head}",
          merges_url: "https://api.github.com/repos/vuejs/vue/merges",
          archive_url:
            "https://api.github.com/repos/vuejs/vue/{archive_format}{/ref}",
          downloads_url: "https://api.github.com/repos/vuejs/vue/downloads",
          issues_url: "https://api.github.com/repos/vuejs/vue/issues{/number}",
          pulls_url: "https://api.github.com/repos/vuejs/vue/pulls{/number}",
          milestones_url:
            "https://api.github.com/repos/vuejs/vue/milestones{/number}",
          notifications_url:
            "https://api.github.com/repos/vuejs/vue/notifications{?since,all,participating}",
          labels_url: "https://api.github.com/repos/vuejs/vue/labels{/name}",
          releases_url: "https://api.github.com/repos/vuejs/vue/releases{/id}",
          deployments_url: "https://api.github.com/repos/vuejs/vue/deployments",
          created_at: "2013-07-29T03:24:51Z",
          updated_at: "2021-10-24T04:30:19Z",
          pushed_at: "2021-10-21T02:58:00Z",
          git_url: "git://github.com/vuejs/vue.git",
          ssh_url: "git@github.com:vuejs/vue.git",
          clone_url: "https://github.com/vuejs/vue.git",
          svn_url: "https://github.com/vuejs/vue",
          homepage: "http://vuejs.org",
          size: 27633,
          stargazers_count: 189584,
          watchers_count: 189584,
          language: "JavaScript",
          has_issues: true,
          has_projects: true,
          has_downloads: true,
          has_wiki: true,
          has_pages: false,
          forks_count: 30473,
          mirror_url: null,
          archived: false,
          disabled: false,
          open_issues_count: 536,
          license: {
            key: "mit",
            name: "MIT License",
            spdx_id: "MIT",
            url: "https://api.github.com/licenses/mit",
            node_id: "MDc6TGljZW5zZTEz",
          },
          allow_forking: true,
          is_template: false,
          topics: ["framework", "frontend", "javascript", "vue"],
          visibility: "public",
          forks: 30473,
          open_issues: 536,
          watchers: 189584,
          default_branch: "dev",
          score: 1,
        },
        {
          id: 2126244,
          node_id: "MDEwOlJlcG9zaXRvcnkyMTI2MjQ0",
          name: "bootstrap",
          full_name: "twbs/bootstrap",
          private: false,
          owner: {
            login: "twbs",
            id: 2918581,
            node_id: "MDEyOk9yZ2FuaXphdGlvbjI5MTg1ODE=",
            avatar_url: "https://avatars.githubusercontent.com/u/2918581?v=4",
            gravatar_id: "",
            url: "https://api.github.com/users/twbs",
            html_url: "https://github.com/twbs",
            followers_url: "https://api.github.com/users/twbs/followers",
            following_url:
              "https://api.github.com/users/twbs/following{/other_user}",
            gists_url: "https://api.github.com/users/twbs/gists{/gist_id}",
            starred_url:
              "https://api.github.com/users/twbs/starred{/owner}{/repo}",
            subscriptions_url:
              "https://api.github.com/users/twbs/subscriptions",
            organizations_url: "https://api.github.com/users/twbs/orgs",
            repos_url: "https://api.github.com/users/twbs/repos",
            events_url: "https://api.github.com/users/twbs/events{/privacy}",
            received_events_url:
              "https://api.github.com/users/twbs/received_events",
            type: "Organization",
            site_admin: false,
          },
          html_url: "https://github.com/twbs/bootstrap",
          description:
            "The most popular HTML, CSS, and JavaScript framework for developing responsive, mobile first projects on the web.",
          fork: false,
          url: "https://api.github.com/repos/twbs/bootstrap",
          forks_url: "https://api.github.com/repos/twbs/bootstrap/forks",
          keys_url: "https://api.github.com/repos/twbs/bootstrap/keys{/key_id}",
          collaborators_url:
            "https://api.github.com/repos/twbs/bootstrap/collaborators{/collaborator}",
          teams_url: "https://api.github.com/repos/twbs/bootstrap/teams",
          hooks_url: "https://api.github.com/repos/twbs/bootstrap/hooks",
          issue_events_url:
            "https://api.github.com/repos/twbs/bootstrap/issues/events{/number}",
          events_url: "https://api.github.com/repos/twbs/bootstrap/events",
          assignees_url:
            "https://api.github.com/repos/twbs/bootstrap/assignees{/user}",
          branches_url:
            "https://api.github.com/repos/twbs/bootstrap/branches{/branch}",
          tags_url: "https://api.github.com/repos/twbs/bootstrap/tags",
          blobs_url:
            "https://api.github.com/repos/twbs/bootstrap/git/blobs{/sha}",
          git_tags_url:
            "https://api.github.com/repos/twbs/bootstrap/git/tags{/sha}",
          git_refs_url:
            "https://api.github.com/repos/twbs/bootstrap/git/refs{/sha}",
          trees_url:
            "https://api.github.com/repos/twbs/bootstrap/git/trees{/sha}",
          statuses_url:
            "https://api.github.com/repos/twbs/bootstrap/statuses/{sha}",
          languages_url:
            "https://api.github.com/repos/twbs/bootstrap/languages",
          stargazers_url:
            "https://api.github.com/repos/twbs/bootstrap/stargazers",
          contributors_url:
            "https://api.github.com/repos/twbs/bootstrap/contributors",
          subscribers_url:
            "https://api.github.com/repos/twbs/bootstrap/subscribers",
          subscription_url:
            "https://api.github.com/repos/twbs/bootstrap/subscription",
          commits_url:
            "https://api.github.com/repos/twbs/bootstrap/commits{/sha}",
          git_commits_url:
            "https://api.github.com/repos/twbs/bootstrap/git/commits{/sha}",
          comments_url:
            "https://api.github.com/repos/twbs/bootstrap/comments{/number}",
          issue_comment_url:
            "https://api.github.com/repos/twbs/bootstrap/issues/comments{/number}",
          contents_url:
            "https://api.github.com/repos/twbs/bootstrap/contents/{+path}",
          compare_url:
            "https://api.github.com/repos/twbs/bootstrap/compare/{base}...{head}",
          merges_url: "https://api.github.com/repos/twbs/bootstrap/merges",
          archive_url:
            "https://api.github.com/repos/twbs/bootstrap/{archive_format}{/ref}",
          downloads_url:
            "https://api.github.com/repos/twbs/bootstrap/downloads",
          issues_url:
            "https://api.github.com/repos/twbs/bootstrap/issues{/number}",
          pulls_url:
            "https://api.github.com/repos/twbs/bootstrap/pulls{/number}",
          milestones_url:
            "https://api.github.com/repos/twbs/bootstrap/milestones{/number}",
          notifications_url:
            "https://api.github.com/repos/twbs/bootstrap/notifications{?since,all,participating}",
          labels_url:
            "https://api.github.com/repos/twbs/bootstrap/labels{/name}",
          releases_url:
            "https://api.github.com/repos/twbs/bootstrap/releases{/id}",
          deployments_url:
            "https://api.github.com/repos/twbs/bootstrap/deployments",
          created_at: "2011-07-29T21:19:00Z",
          updated_at: "2021-10-24T04:27:57Z",
          pushed_at: "2021-10-23T07:53:27Z",
          git_url: "git://github.com/twbs/bootstrap.git",
          ssh_url: "git@github.com:twbs/bootstrap.git",
          clone_url: "https://github.com/twbs/bootstrap.git",
          svn_url: "https://github.com/twbs/bootstrap",
          homepage: "https://getbootstrap.com",
          size: 192284,
          stargazers_count: 153533,
          watchers_count: 153533,
          language: "JavaScript",
          has_issues: true,
          has_projects: true,
          has_downloads: true,
          has_wiki: false,
          has_pages: true,
          forks_count: 75054,
          mirror_url: null,
          archived: false,
          disabled: false,
          open_issues_count: 432,
          license: {
            key: "mit",
            name: "MIT License",
            spdx_id: "MIT",
            url: "https://api.github.com/licenses/mit",
            node_id: "MDc6TGljZW5zZTEz",
          },
          allow_forking: true,
          is_template: false,
          topics: [
            "bootstrap",
            "css",
            "css-framework",
            "html",
            "javascript",
            "sass",
            "scss",
          ],
          visibility: "public",
          forks: 75054,
          open_issues: 432,
          watchers: 153533,
          default_branch: "main",
          score: 1,
        },
      ],
    };
  },
  mounted() {
    this.renderChart(this.chartdata, this.options);
  },
};
</script>


