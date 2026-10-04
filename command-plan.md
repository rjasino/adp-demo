## Instruction to Create Commands

## Commands

- name: `/generate-script`
- description: infer from the conversation
- usage:
  - `/generate-script Generate script from the conversation`
- steps:
  - Receive the conversation from the user.
  - Use agent skill to perform the task.
  - Generate a script based on the analysis.
- definition of done:
  - the script is generated in `docs\scripts\<slug>`.

---

- name: `/write-socmed-post`
- description: infer from the conversation
- usage:
  - `/write-socmed-post Generate social media post from the generated script.`
- steps:
  - Read the script in the designated directory.
  - Use agent skill to perform the task.
  - Generate the social media post and save it to the designated directory.
- definition of done:
  - the social media post is save in `docs\post\<slug>`.
