### Методы работы с кусками


getById(int $id): Offcut;

findByIds($ids) array;

findByExternalId(int $offcutId, bool $active = true): ?Offcut;

findByDate($sdate, $edate, int $statusTransition);

findWaitingRecieve();

findByStatus($status, $gFilter = []);

findWaitingRelease();

onStore($gids = []);

findByGood($gid);

findUsedInOrder(int $orderId);

findCreatedByOrder(int $orderId);

add(Offcut $offcut);

resetByOrder(int $orderId);

findFirstWithParams(int $goodsId, int $length, int $width, OffcutStatus $status = null);

existForOrder(int $orderId): bool;

findChildren(): array;