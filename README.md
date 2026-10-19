Prime_tennis

## Supabase keepalive (송도테니스 장바구니 도우미 대시보드)
`.github/workflows/supabase-keepalive.yml`이 3일마다 Supabase `keepalive()`를 불러 무료 프로젝트가 멈추지 않게 합니다.

처음 한 번: 저장소 **Settings → Secrets and variables → Actions → New repository secret**에 두 개를 넣으세요.
- `SUPABASE_URL`: `https://<프로젝트>.supabase.co`
- `SUPABASE_KEY`: `sb_publishable_...` 공개 키

넣은 뒤 **Actions → Supabase keepalive → Run workflow**로 한 번 실행해 초록색(성공)인지 확인하세요.
Supabase에는 프로그램 폴더의 `supabase/setup.sql` 최신본이 실행돼 있어야 합니다(`keepalive` 함수 포함).
