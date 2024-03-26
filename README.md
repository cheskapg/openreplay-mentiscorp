# **How to run frontend locally**

## _Step by step guide_

---

1. Open your terminal.
2. Clone the repository by running the following command:

```bash
git clone https://github.com/NicoTuban30/openreplay-mentiscorp.git
```

3. Navigate to the cloned repository:

```bash
cd openreplay
```

4. Then, navigate to the frontend directory:

```bash
cd frontend
```

5. Now, you're in the frontend directory. Install the necessary dependencies using Yarn. If you don't have Yarn installed, you can get it [here](https://classic.yarnpkg.com/en/docs/install/). Run the following command to install the dependencies:

```bash
yarn install
```

6. Next, you need to configure the mode in the `webpack.config.ts` file. By default, the mode is commented out. You need to uncomment it.

Find the following line in the `webpack.config.ts` file:

```typescript
// mode: isDevelopment ? "development" : "production",
```

Uncomment it to look like this:

```typescript
mode: isDevelopment ? "development" : "production",
```

7. Now, you need to create a `.env` file to set your environment variables. In the root of the frontend directory, create a new file named `.env`.

Add the following line to the `.env` file:

```bash
NODE_ENV=development
```

8. Finally, you can start the application. In the terminal, make sure you're still in the frontend directory, then run the following command:

```bash
yarn start
```
