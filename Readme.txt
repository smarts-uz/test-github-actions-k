gh run download 16769894868 --name hello-artifact



gh attestation download hello.txt -R smarts-uz/test-github-actions-k



gh attestation trusted-root > trusted_root.jsonl


gh attestation verify hello.txt `
  -R smarts-uz/test-github-actions-k `
  --bundle sha256-0e99fab80b0bfc342c49c0c0d56ce28e7c36c4ecbae2375422ad199a5d81c844.jsonl `
  --custom-trusted-root trusted_root.jsonl

