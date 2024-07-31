# 기본 Node.js 이미지 사용
FROM node:18-alpine

WORKDIR /app

# 필요한 파일 복사 및 npm 패키지 설치
COPY package.json package-lock.json ./
RUN npm install --legacy-peer-deps


# 필요한 파일만 복사
COPY .next ./.next
COPY public ./public

# 포트 설정
EXPOSE 3000

# 앱 실행
CMD ["npm", "start"]