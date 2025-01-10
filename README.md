# What is this?

The github.dev web-based editor is a lightweight editing experience that runs entirely in your browser. You can navigate files and source code repositories from GitHub, and make and commit code changes.

There are two ways to go directly to a VS Code environment in your browser and start coding:
12345678


* Press the . key on any repository or pull request.
* Swap `.com` with `.dev` in the URL. For example, this repo https://github.com/github/dev becomes http://github.dev/github/dev

Preview the gif below to get a quick demo of github.dev in action.
# $$


$$

# Why?
It’s a quick way to edit and navigate code. It's especially useful if you want to edit multiple files at a time or take advantage of all the powerful code editing features of Visual Studio Code when making a quick change. For more information, see our [documentation][def].



jobs:
  upload:
      runs-on: ubuntu-latest
          steps:
                - name: Create a file
                        run: echo "hello world" > my-file.txt
                              - name: Upload Artifact
                                      uses: actions/upload-artifact@v3
                                              with:
                                                        name: my-artifact # NOTE: same artifact name
                                                                  path: my-file.txt
                                                                    upload-again:
                                                                        needs: upload
                                                                            runs-on: ubuntu-latest
                                                                                steps:
                                                                                      - name: Create a different file
                                                                                              run: echo "goodbye world" > my-file.txt
                                                                                                    - name: Upload Artifact
                                                                                                            uses: actions/upload-artifact@v3
                                                                                                                    with:
                                                                                                                              name: my-artifact # NOTE: same artifact name
                                                                                                                                        path: my-file.txt

upload:
                                                                                                                                              runs-on: ubuntu-latest
                                                                                                                                                  steps:
                                                                                                                                                        - name: Create a file
                                                                                                                                                                run: echo "hello world" > my-file.txt
                                                                                                                                                                      - name: Upload Artifact
                                                                                                                                                                              uses: actions/upload-artifact@v3
                                                                                                                                                                                      with:
                                                                                                                                                                                                name: my-artifact # NOTE: same artifact name
                                                                                                                                                                                                          path: my-file.txt
                                                                                                                                                                                                            upload-again:
                                                                                                                                                                                                                needs: upload
                                                                                                                                                                                                                    runs-on: ubuntu-latest

- name: Create a different file
                                                                                                                                                                                                                                      run: echo "goodbye world" > my-file.txt
                                                                                                                                                                                                                                            - name: Upload Artifact
                                                                                                                                                                                                                                                    uses: actions/upload-artifact@v3
                                                                                                
                                                                                                with:
                                                                                                                                                                                                                                                                      name: my-artifact # NOTE: same artifact name
                                                                                                                                                                                                                                                                                path: my-file.txt
