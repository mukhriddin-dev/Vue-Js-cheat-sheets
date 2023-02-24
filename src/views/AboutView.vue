<template>
  <div class="about">

    <div class="container">
      <div class="card">
        <div class="card-wrapper">
          <div class="card-item">
            <figure class="card-image">
              <img src="https://telegra.ph/file/dad08c7a7ab9099efc8d8.jpg" alt="...">
            </figure>
            <a class="card-content" target="_blank" href="https://instagram.com/mukhriddin_web">
              <span class="card-tags">Follow</span>
              <h2 class="card-title">Get the Ultimate Vue Cheat Sheet </h2>
              <footer class="card-footer">
                <div class="card-user">
                  
                  <figure class="card-user-img">
                    <img src="https://telegra.ph/file/5384ea9531529dab7c7a9.jpg" alt="...">
                  </figure>
                  <span class="card-user-name">mukhriddin_web</span>
                </div>
                <time class="card-time">
                  <svg class="icon icon-time">
                    <use xlink:href="#icon-time"></use>
                  </svg>
                  Feb 24, 2023
                </time>
                <span class="card-comment">
                  <svg class="icon icon-comment">
                    <use xlink:href="#icon-comment"></use>
                  </svg>
                  12
                </span>
              </footer>
            </a>
          </div>
        </div>
      </div>
    </div>

    <svg style="position: absolute; width: 0; height: 0; overflow: hidden;" version="1.1"
      xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
      <defs>
        <symbol id="icon-comment" viewBox="0 0 24 24">
          <path fill="none" d="M0 0h24v24H0z" />
          <path
            d="M5.455 15L1 18.5V3a1 1 0 0 1 1-1h15a1 1 0 0 1 1 1v12H5.455zm-.692-2H16V4H3v10.385L4.763 13zM8 17h10.237L20 18.385V8h1a1 1 0 0 1 1 1v13.5L17.545 19H9a1 1 0 0 1-1-1v-1z" />
        </symbol>

        <symbol id="icon-time" viewBox="0 0 24 24">
          <path fill="none" d="M0 0h24v24H0z" />
          <path
            d="M12 22C6.477 22 2 17.523 2 12S6.477 2 12 2s10 4.477 10 10-4.477 10-10 10zm0-2a8 8 0 1 0 0-16 8 8 0 0 0 0 16zm1-8h4v2h-6V7h2v5z" />
        </symbol>
      </defs>
    </svg>



  </div>
</template>

<style scoped lang="scss">

* {
	box-sizing: border-box;
	margin: 0;
	padding: 0;
}

a {
	text-decoration: none;
}

body {
	font-family: sans-serif;
	font-size: 16px;
	display: grid;
	place-items: center center;
	width: 100%;
	height: 100vh;
}

.icon {
	width: 1em;
	height: 1em;
	display: inline-block;
	fill: currentcolor;
}

.card {
	&-wrapper {
		position: relative;
	}

	&-item {
		width: 450px;
		height: 540px;
		position: relative;
		border-radius: 32px;
		overflow: hidden;

		&:hover {
			.card-image:after {
				background: linear-gradient(
					180deg,
					rgba(0, 0, 0, 0) 10%,
					rgba(0, 0, 0, 0.7) 50%,
					rgba(0, 0, 0, 0.9) 100%
				);
			}

			.card-image {
				img {
					transform: scale(1.03);
				}
			}
		}

		.card-image {
			width: 100%;
			height: 100%;
			overflow: hiddden;
			position: relative;

			&:after {
				content: "";
				width: 100%;
				height: 100%;
				display: block;
				position: absolute;
				top: 0;
				background: rgb(0, 0, 0);
				background: linear-gradient(
					180deg,
					rgba(0, 0, 0, 0) 10%,
					rgba(0, 0, 0, 0.7) 72%,
					rgba(0, 0, 0, 0.9) 100%
				);
			}

			img {
				width: 100%;
				height: 100%;
				object-fit: cover;
				transition: 0.4s;
			}
		}

		.card-content {
			width: 100%;
			height: 100%;
			z-index: 1;
			position: absolute;
			top: 0;
			padding: 40px;
			display: flex;
			flex-direction: column;
			justify-content: flex-end;
			row-gap: 20px;

			.card-tags {
				padding: 10px 20px;
				background-color: #ff0984;
				border-radius: 100px;
				color: #fff;
				font-size: 12px;
				width: max-content;
				letter-spacing: 0.6px;
			}

			.card-title {
				font-size: 24px;
				color: #fff;
				font-weight: bold;
				line-height: 1.4;
			}

			.card-footer {
				display: flex;
				align-items: center;
				column-gap: 20px;
				font-size: 14px;
				color: #fff;

				.card-user {
					display: flex;
					align-items: center;
					column-gap: 8px;

					&-img {
						width: 36px;
						height: 36px;
						min-width: 36px;
						max-width: 36px;
						overflow: hidden;
						border-radius: 100px;

						img {
							width: 100%;
							height: 100%;
							object-fit: cover;
						}
					}
				}

				.card-time,
				.card-comment {
					display: flex;
					align-items: center;
					column-gap: 8px;

					.icon {
						color: #e1a00f;
					}
				}
			}
		}
	}
}

@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}</style>
